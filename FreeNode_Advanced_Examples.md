# FreeNode - продвинутые примеры использования

Класс `FreeNode` представляет узел с абсолютными координатами в T-Flex CAD API. Это один из фундаментальных классов для создания геометрических конструкций.

## Продвинутые примеры использования

### 1. Создание массива узлов с использованием циклов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание массива узлов");

// Создание двумерного массива узлов
int rows = 5;
int cols = 8;
double spacing = 10.0;
FreeNode[,] nodeArray = new FreeNode[rows, cols];

for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols; j++)
    {
        // Создание узла с координатами
        nodeArray[i, j] = new FreeNode(document, j * spacing, i * spacing);
        
        // Дополнительная настройка узла (например, привязка к сетке)
        // nodeArray[i, j].SnapToGrid = true;
    }
}

// Создание линий между узлами для визуализации массива
for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols - 1; j++)
    {
        LineConstruction line = new LineConstruction(document);
        line.SetTwoNodes(nodeArray[i, j], nodeArray[i, j + 1]);
        line.Color = 12632256; // Серый цвет
    }
}

for (int i = 0; i < rows - 1; i++)
{
    for (int j = 0; j < cols; j++)
    {
        LineConstruction line = new LineConstruction(document);
        line.SetTwoNodes(nodeArray[i, j], nodeArray[i + 1, j]);
        line.Color = 12632256; // Серый цвет
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание узлов на основе математических функций

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание узлов на основе функций");

// Создание узлов для синусоиды
int pointCount = 20;
double amplitude = 20.0;
double frequency = 0.5;
double spacing = 5.0;

FreeNode[] sineNodes = new FreeNode[pointCount];

for (int i = 0; i < pointCount; i++)
{
    double x = i * spacing;
    double y = amplitude * Math.Sin(frequency * x * Math.PI / 180.0);
    sineNodes[i] = new FreeNode(document, x, y);
}

// Соединение узлов линиями для создания кривой
for (int i = 0; i < pointCount - 1; i++)
{
    LineConstruction line = new LineConstruction(document);
    line.SetTwoNodes(sineNodes[i], sineNodes[i + 1]);
    line.Color = 255; // Красный цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание узлов с использованием геометрических расчетов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание узлов с геометрическими расчетами");

// Создание правильного многоугольника
int sides = 8;
double radius = 30.0;
double centerX = 50.0;
double centerY = 50.0;

FreeNode[] polygonNodes = new FreeNode[sides];

for (int i = 0; i < sides; i++)
{
    double angle = 2 * Math.PI * i / sides;
    double x = centerX + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    polygonNodes[i] = new FreeNode(document, x, y);
}

// Создание линий многоугольника
for (int i = 0; i < sides; i++)
{
    LineConstruction line = new LineConstruction(document);
    line.SetTwoNodes(polygonNodes[i], polygonNodes[(i + 1) % sides]);
    line.Color = 65280; // Зеленый цвет
}

// Создание узлов на пересечении диагоналей
FreeNode[] diagonalNodes = new FreeNode[sides * (sides - 3) / 2];
int nodeIndex = 0;

for (int i = 0; i < sides - 2; i++)
{
    for (int j = i + 2; j < sides; j++)
    {
        if (!(i == 0 && j == sides - 1)) // Исключаем стороны многоугольника
        {
            // В реальной реализации здесь потребуется вычисление точки пересечения
            // Для упрощения примера используем центр многоугольника
            diagonalNodes[nodeIndex] = new FreeNode(document, centerX, centerY);
            nodeIndex++;
        }
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция с другими объектами и сложные конструкции

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция узлов с другими объектами");

// Создание системы связанных узлов
FreeNode centerNode = new FreeNode(document, 50, 50);
FreeNode[] orbitNodes = new FreeNode[6];
FreeNode[] satelliteNodes = new FreeNode[6];

// Создание узлов по орбите
for (int i = 0; i < 6; i++)
{
    double angle = 2 * Math.PI * i / 6;
    double radius = 30.0;
    double x = centerNode.X.Value + radius * Math.Cos(angle);
    double y = centerNode.Y.Value + radius * Math.Sin(angle);
    orbitNodes[i] = new FreeNode(document, x, y);
    
    // Создание спутников на большем радиусе
    double satelliteRadius = 50.0;
    double satX = centerNode.X.Value + satelliteRadius * Math.Cos(angle);
    double satY = centerNode.Y.Value + satelliteRadius * Math.Sin(angle);
    satelliteNodes[i] = new FreeNode(document, satX, satY);
}

// Создание линий от центра к орбитальным узлам
for (int i = 0; i < 6; i++)
{
    LineConstruction line = new LineConstruction(document);
    line.SetTwoNodes(centerNode, orbitNodes[i]);
    line.Color = 16711680; // Синий цвет
}

// Создание линий от орбитальных узлов к спутникам
for (int i = 0; i < 6; i++)
{
    LineConstruction line = new LineConstruction(document);
    line.SetTwoNodes(orbitNodes[i], satelliteNodes[i]);
    line.Color = 65535; // Голубой цвет
}

// Создание окружностей вокруг спутников
for (int i = 0; i < 6; i++)
{
    CircleConstruction circle = new CircleConstruction(document);
    circle.SetCenterAndRadius(satelliteNodes[i], 5.0);
    circle.Color = 16711935; // Пурпурный цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством узлов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества узлов с минимальными вызовами API
int nodeCount = 1000;
FreeNode[] nodes = new FreeNode[nodeCount];

// Предварительное вычисление координат
double[] xCoords = new double[nodeCount];
double[] yCoords = new double[nodeCount];

Random random = new Random();
for (int i = 0; i < nodeCount; i++)
{
    xCoords[i] = random.NextDouble() * 200; // X от 0 до 200
    yCoords[i] = random.NextDouble() * 150; // Y от 0 до 150
}

// Создание узлов
for (int i = 0; i < nodeCount; i++)
{
    nodes[i] = new FreeNode(document, xCoords[i], yCoords[i]);
}

// Создание соединений между ближайшими узлами
for (int i = 0; i < nodeCount; i++)
{
    // Находим 3 ближайших узла
    List<Tuple<double, int>> distances = new List<Tuple<double, int>>();
    
    for (int j = 0; j < nodeCount; j++)
    {
        if (i != j)
        {
            double dx = nodes[i].X.Value - nodes[j].X.Value;
            double dy = nodes[i].Y.Value - nodes[j].Y.Value;
            double distance = Math.Sqrt(dx * dx + dy * dy);
            distances.Add(new Tuple<double, int>(distance, j));
        }
    }
    
    // Сортируем по расстоянию и берем 3 ближайших
    distances.Sort((a, b) => a.Item1.CompareTo(b.Item1));
    
    for (int k = 0; k < Math.Min(3, distances.Count); k++)
    {
        int j = distances[k].Item2;
        LineConstruction line = new LineConstruction(document);
        line.SetTwoNodes(nodes[i], nodes[j]);
        line.Color = 12632256; // Серый цвет
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими узлами и обновление координат

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические узлы");

// Создание узлов с возможностью динамического обновления
FreeNode dynamicNode1 = new FreeNode(document, 30, 30);
FreeNode dynamicNode2 = new FreeNode(document, 70, 70);

// Создание линии между узлами
LineConstruction dynamicLine = new LineConstruction(document);
dynamicLine.SetTwoNodes(dynamicNode1, dynamicNode2);
dynamicLine.Color = 255; // Красный цвет

// Создание узла, который будет двигаться по круговой траектории
FreeNode movingNode = new FreeNode(document, 50, 50);
CircleConstruction trajectory = new CircleConstruction(document);
trajectory.SetCenterAndRadius(new FreeNode(document, 50, 50), 30);
trajectory.Color = 12632256; // Серый цвет

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления координат узлов
// Например, в обработчике таймера или событий:
/*
public void UpdateMovingNode(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление движущегося узла");
    
    double angle = time * 0.1; // Скорость движения
    double centerX = 50;
    double centerY = 50;
    double radius = 30;
    
    double newX = centerX + radius * Math.Cos(angle);
    double newY = centerY + radius * Math.Sin(angle);
    
    // Обновление координат узла
    movingNode.X.Value = newX;
    movingNode.Y.Value = newY;
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
```

## Свойства и методы

### Основные свойства:

- `X` - Координата X узла
- `Y` - Координата Y узла
- `SnapToGrid` - Привязка к сетке (если поддерживается)
- `Constraints` - Ограничения на перемещение (если поддерживается)

### Унаследованные свойства от Node:

- `IsFixed` - Фиксирован ли узел
- `IsConstructionNode` - Является ли узлом построения
- `IsOutlineNode` - Является ли узлом контура

## Заключение

Продвинутое использование класса `FreeNode` включает в себя создание сложных геометрических конструкций, работу с массивами узлов, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами узлов важно учитывать производительность и использовать эффективные алгоритмы для вычисления координат и установления связей между узлами.
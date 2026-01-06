# PathConstruction - продвинутые примеры использования

Класс `PathConstruction` представляет контур построения в T-Flex CAD API. Этот класс предоставляет возможности для создания сложных контуров, состоящих из различных сегментов.

## Продвинутые примеры использования

### 1. Создание сложных контуров с множеством сегментов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сложных контуров");

// Создание контура в форме сложного многоугольника
PathConstruction complexPath = new PathConstruction(document);

// Создание узлов для сложного многоугольника
FreeNode[] complexNodes = new FreeNode[12];
double centerX = 50;
double centerY = 50;
double outerRadius = 30;
double innerRadius = 15;

for (int i = 0; i < 12; i++)
{
    double angle = 2 * Math.PI * i / 12;
    double radius = (i % 2 == 0) ? outerRadius : innerRadius;
    double x = centerX + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    complexNodes[i] = new FreeNode(document, x, y);
}

// Добавление сегментов в контур
for (int i = 0; i < 12; i++)
{
    complexPath.AddSegment(complexNodes[i], complexNodes[(i + 1) % 12]);
}

complexPath.Color = 255; // Красный цвет

// Создание контура с закругленными углами
PathConstruction roundedPath = new PathConstruction(document);

// Создание узлов для прямоугольника
FreeNode[] rectNodes = new FreeNode[4];
rectNodes[0] = new FreeNode(document, 100, 30);
rectNodes[1] = new FreeNode(document, 140, 30);
rectNodes[2] = new FreeNode(document, 140, 70);
rectNodes[3] = new FreeNode(document, 100, 70);

// Добавление сегментов с закруглениями
double cornerRadius = 5;
for (int i = 0; i < 4; i++)
{
    FreeNode startNode = rectNodes[i];
    FreeNode endNode = rectNodes[(i + 1) % 4];
    
    // Создание промежуточных точек для закругления
    FreeNode control1, control2;
    
    if (i == 0) // Нижняя сторона
    {
        control1 = new FreeNode(document, startNode.X.Value + cornerRadius, startNode.Y.Value);
        control2 = new FreeNode(document, endNode.X.Value, endNode.Y.Value + cornerRadius);
    }
    else if (i == 1) // Правая сторона
    {
        control1 = new FreeNode(document, startNode.X.Value, startNode.Y.Value + cornerRadius);
        control2 = new FreeNode(document, endNode.X.Value - cornerRadius, endNode.Y.Value);
    }
    else if (i == 2) // Верхняя сторона
    {
        control1 = new FreeNode(document, startNode.X.Value - cornerRadius, startNode.Y.Value);
        control2 = new FreeNode(document, endNode.X.Value, endNode.Y.Value - cornerRadius);
    }
    else // Левая сторона
    {
        control1 = new FreeNode(document, startNode.X.Value, startNode.Y.Value - cornerRadius);
        control2 = new FreeNode(document, endNode.X.Value + cornerRadius, endNode.Y.Value);
    }
    
    // Добавление сегментов
    roundedPath.AddSegment(startNode, control1);
    roundedPath.AddSegment(control1, control2);
    roundedPath.AddSegment(control2, endNode);
}

roundedPath.Color = 65280; // Зеленый цвет

// Создание контура с вырезами
PathConstruction pathWithCutouts = new PathConstruction(document);

// Создание внешнего контура
FreeNode[] outerNodes = new FreeNode[4];
outerNodes[0] = new FreeNode(document, 30, 100);
outerNodes[1] = new FreeNode(document, 80, 100);
outerNodes[2] = new FreeNode(document, 80, 150);
outerNodes[3] = new FreeNode(document, 30, 150);

for (int i = 0; i < 4; i++)
{
    pathWithCutouts.AddSegment(outerNodes[i], outerNodes[(i + 1) % 4]);
}

// Создание внутренних контуров (вырезов)
FreeNode[] cutout1Nodes = new FreeNode[4];
cutout1Nodes[0] = new FreeNode(document, 40, 110);
cutout1Nodes[1] = new FreeNode(document, 50, 110);
cutout1Nodes[2] = new FreeNode(document, 50, 120);
cutout1Nodes[3] = new FreeNode(document, 40, 120);

for (int i = 0; i < 4; i++)
{
    pathWithCutouts.AddSegment(cutout1Nodes[i], cutout1Nodes[(i + 1) % 4]);
}

FreeNode[] cutout2Nodes = new FreeNode[4];
cutout2Nodes[0] = new FreeNode(document, 60, 130);
cutout2Nodes[1] = new FreeNode(document, 70, 130);
cutout2Nodes[2] = new FreeNode(document, 70, 140);
cutout2Nodes[3] = new FreeNode(document, 60, 140);

for (int i = 0; i < 4; i++)
{
    pathWithCutouts.AddSegment(cutout2Nodes[i], cutout2Nodes[(i + 1) % 4]);
}

pathWithCutouts.Color = 16711680; // Синий цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание контуров с геометрическими расчетами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание контуров с геометрическими расчетами");

// Создание контура в форме правильного многоугольника
PathConstruction polygonPath = new PathConstruction(document);

int sides = 8;
double radius = 25;
double centerX = 50;
double centerY = 50;

FreeNode[] polygonNodes = new FreeNode[sides];

for (int i = 0; i < sides; i++)
{
    double angle = 2 * Math.PI * i / sides - Math.PI / 2; // Начинаем с вершины
    double x = centerX + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    polygonNodes[i] = new FreeNode(document, x, y);
}

for (int i = 0; i < sides; i++)
{
    polygonPath.AddSegment(polygonNodes[i], polygonNodes[(i + 1) % sides]);
}

polygonPath.Color = 255; // Красный цвет

// Создание контура в форме звезды
PathConstruction starPath = new PathConstruction(document);

int starPoints = 10;
double outerRadius = 30;
double innerRadius = 15;
double starCenterX = 120;
double starCenterY = 50;

FreeNode[] starNodes = new FreeNode[starPoints];

for (int i = 0; i < starPoints; i++)
{
    double radius = (i % 2 == 0) ? outerRadius : innerRadius;
    double angle = 2 * Math.PI * i / starPoints - Math.PI / 2;
    double x = starCenterX + radius * Math.Cos(angle);
    double y = starCenterY + radius * Math.Sin(angle);
    starNodes[i] = new FreeNode(document, x, y);
}

for (int i = 0; i < starPoints; i++)
{
    starPath.AddSegment(starNodes[i], starNodes[(i + 1) % starPoints]);
}

starPath.Color = 65280; // Зеленый цвет

// Создание контура с касательными к окружности
PathConstruction tangentPath = new PathConstruction(document);

double circleRadius = 20;
FreeNode circleCenter = new FreeNode(document, 50, 120);

// Создание окружности для визуализации
CircleConstruction referenceCircle = new CircleConstruction(document);
referenceCircle.SetCenterAndRadius(circleCenter, circleRadius);
referenceCircle.Color = 12632256; // Серый цвет

// Создание точек касания
int tangentPoints = 8;
FreeNode[] tangentNodes = new FreeNode[tangentPoints];

for (int i = 0; i < tangentPoints; i++)
{
    double angle = 2 * Math.PI * i / tangentPoints;
    double x = circleCenter.X.Value + circleRadius * Math.Cos(angle);
    double y = circleCenter.Y.Value + circleRadius * Math.Sin(angle);
    tangentNodes[i] = new FreeNode(document, x, y);
}

// Создание контура с касательными сегментами
for (int i = 0; i < tangentPoints; i++)
{
    // Создание касательной линии (приблизительно)
    double tangentLength = 15;
    double tangentAngle = angle + Math.PI / 2;
    double tangentX = tangentNodes[i].X.Value + tangentLength * Math.Cos(tangentAngle);
    double tangentY = tangentNodes[i].Y.Value + tangentLength * Math.Sin(tangentAngle);
    FreeNode tangentPoint = new FreeNode(document, tangentX, tangentY);
    
    tangentPath.AddSegment(tangentNodes[i], tangentPoint);
    
    // Создание визуального маркера точки касания
    CircleConstruction marker = new CircleConstruction(document);
    marker.SetCenterAndRadius(tangentNodes[i], 1);
    marker.Color = 16776960; // Желтый цвет
}

tangentPath.Color = 16711680; // Синий цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание контуров с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы контуров");

// Создание системы контуров в форме сетки
int rows = 4;
int cols = 5;
double spacingX = 25.0;
double spacingY = 20.0;
double cellWidth = 20.0;
double cellHeight = 15.0;
double startX = 20.0;
double startY = 20.0;

PathConstruction[,] gridPaths = new PathConstruction[rows, cols];

for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols; j++)
    {
        gridPaths[i, j] = new PathConstruction(document);
        
        // Вычисление координат ячейки
        double cellX = startX + j * spacingX;
        double cellY = startY + i * spacingY;
        
        // Создание узлов для прямоугольной ячейки
        FreeNode[] cellNodes = new FreeNode[4];
        cellNodes[0] = new FreeNode(document, cellX, cellY);
        cellNodes[1] = new FreeNode(document, cellX + cellWidth, cellY);
        cellNodes[2] = new FreeNode(document, cellX + cellWidth, cellY + cellHeight);
        cellNodes[3] = new FreeNode(document, cellX, cellY + cellHeight);
        
        // Добавление сегментов
        for (int k = 0; k < 4; k++)
        {
            gridPaths[i, j].AddSegment(cellNodes[k], cellNodes[(k + 1) % 4]);
        }
        
        // Установка цвета с градиентом
        int red = (int)(255 * (double)i / (rows - 1));
        int green = (int)(255 * (double)j / (cols - 1));
        int blue = 255 - (red + green) / 2;
        gridPaths[i, j].Color = (red << 16) | (green << 8) | blue;
        
        // Установка толщины линии
        gridPaths[i, j].LineWidth = 1 + (i + j) / 4;
    }
}

// Создание контуров с переменной формой
int variablePaths = 6;
PathConstruction[] variablePathsArray = new PathConstruction[variablePaths];

for (int i = 0; i < variablePaths; i++)
{
    variablePathsArray[i] = new PathConstruction(document);
    
    double centerX = 150 + i * 30;
    double centerY = 30 + i * 15;
    int sides = 3 + i; // От треугольника до восьмиугольника
    double radius = 10 + i * 2;
    
    FreeNode[] nodes = new FreeNode[sides];
    
    for (int j = 0; j < sides; j++)
    {
        double angle = 2 * Math.PI * j / sides - Math.PI / 2;
        double x = centerX + radius * Math.Cos(angle);
        double y = centerY + radius * Math.Sin(angle);
        nodes[j] = new FreeNode(document, x, y);
    }
    
    for (int j = 0; j < sides; j++)
    {
        variablePathsArray[i].AddSegment(nodes[j], nodes[(j + 1) % sides]);
    }
    
    variablePathsArray[i].Color = 16711935; // Пурпурный цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция контуров с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция контуров с другими объектами");

// Создание контура и связанных объектов
PathConstruction mainPath = new PathConstruction(document);

// Создание контура в форме неправильного многоугольника
FreeNode[] mainNodes = new FreeNode[7];
mainNodes[0] = new FreeNode(document, 40, 40);
mainNodes[1] = new FreeNode(document, 70, 35);
mainNodes[2] = new FreeNode(document, 80, 60);
mainNodes[3] = new FreeNode(document, 65, 80);
mainNodes[4] = new FreeNode(document, 45, 75);
mainNodes[5] = new FreeNode(document, 35, 60);
mainNodes[6] = new FreeNode(document, 30, 50);

for (int i = 0; i < 7; i++)
{
    mainPath.AddSegment(mainNodes[i], mainNodes[(i + 1) % 7]);
}

mainPath.Color = 255; // Красный цвет

// Создание точек на контуре
int pointsOnPath = 12;
FreeNode[] pathPoints = new FreeNode[pointsOnPath];

for (int i = 0; i < pointsOnPath; i++)
{
    // В реальной реализации здесь потребуется вычисление точек на контуре
    // Для упрощения примера создаем точки вручную
    double t = (double)i / (pointsOnPath - 1);
    int segmentIndex = (int)(t * 7);
    double segmentT = (t * 7) - segmentIndex;
    
    double x = mainNodes[segmentIndex].X.Value + 
              segmentT * (mainNodes[(segmentIndex + 1) % 7].X.Value - mainNodes[segmentIndex].X.Value);
    double y = mainNodes[segmentIndex].Y.Value + 
              segmentT * (mainNodes[(segmentIndex + 1) % 7].Y.Value - mainNodes[segmentIndex].Y.Value);
    
    pathPoints[i] = new FreeNode(document, x, y);
    
    // Создание визуальных маркеров точек
    CircleConstruction pointMarker = new CircleConstruction(document);
    pointMarker.SetCenterAndRadius(pathPoints[i], 1.5);
    pointMarker.Color = 65280; // Зеленый цвет
}

// Создание нормалей к контуру
int normalsCount = 6;
LineConstruction[] normals = new LineConstruction[normalsCount];

for (int i = 0; i < normalsCount; i++)
{
    int pointIndex = i * pointsOnPath / (normalsCount - 1);
    if (pointIndex >= pointsOnPath) pointIndex = pointsOnPath - 1;
    
    FreeNode point = pathPoints[pointIndex];
    
    // Вычисление направления нормали (приблизительно)
    double normalLength = 10;
    double normalAngle = Math.PI / 3 * Math.Sin(2 * Math.PI * i / (normalsCount - 1));
    double endX = point.X.Value + normalLength * Math.Cos(normalAngle);
    double endY = point.Y.Value + normalLength * Math.Sin(normalAngle);
    
    FreeNode endPoint = new FreeNode(document, endX, endY);
    normals[i] = new LineConstruction(document);
    normals[i].SetTwoNodes(point, endPoint);
    normals[i].Color = 16711680; // Синий цвет
}

// Создание контура, описывающего исходный контур
PathConstruction boundingPath = new PathConstruction(document);

// Вычисление ограничивающего прямоугольника
double minX = mainNodes[0].X.Value, maxX = mainNodes[0].X.Value;
double minY = mainNodes[0].Y.Value, maxY = mainNodes[0].Y.Value;

for (int i = 1; i < 7; i++)
{
    if (mainNodes[i].X.Value < minX) minX = mainNodes[i].X.Value;
    if (mainNodes[i].X.Value > maxX) maxX = mainNodes[i].X.Value;
    if (mainNodes[i].Y.Value < minY) minY = mainNodes[i].Y.Value;
    if (mainNodes[i].Y.Value > maxY) maxY = mainNodes[i].Y.Value;
}

// Создание узлов ограничивающего прямоугольника
FreeNode[] boundingNodes = new FreeNode[4];
boundingNodes[0] = new FreeNode(document, minX - 5, minY - 5);
boundingNodes[1] = new FreeNode(document, maxX + 5, minY - 5);
boundingNodes[2] = new FreeNode(document, maxX + 5, maxY + 5);
boundingNodes[3] = new FreeNode(document, minX - 5, maxY + 5);

for (int i = 0; i < 4; i++)
{
    boundingPath.AddSegment(boundingNodes[i], boundingNodes[(i + 1) % 4]);
}

boundingPath.Color = 16776960; // Желтый цвет
boundingPath.Style = LineStyle.Dash; // Пунктирная линия

// Создание контура, вписанного в исходный контур
PathConstruction inscribedPath = new PathConstruction(document);

// Создание уменьшенной версии исходного контура
for (int i = 0; i < 7; i++)
{
    double centerX = 55; // Центр исходного контура
    double centerY = 60;
    double scale = 0.7;
    
    double x = centerX + (mainNodes[i].X.Value - centerX) * scale;
    double y = centerY + (mainNodes[i].Y.Value - centerY) * scale;
    
    FreeNode newNode = new FreeNode(document, x, y);
    mainNodes[i] = newNode; // Обновляем ссылки на узлы
}

for (int i = 0; i < 7; i++)
{
    inscribedPath.AddSegment(mainNodes[i], mainNodes[(i + 1) % 7]);
}

inscribedPath.Color = 16711935; // Пурпурный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством контуров

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества контуров с минимальными вызовами API
int pathCount = 100;
PathConstruction[] paths = new PathConstruction[pathCount];

// Предварительное создание узлов
int nodesPerPath = 4;
FreeNode[,] allNodes = new FreeNode[pathCount, nodesPerPath];

Random random = new Random();
for (int i = 0; i < pathCount; i++)
{
    double baseX = 20 + random.NextDouble() * 160;
    double baseY = 20 + random.NextDouble() * 110;
    
    for (int j = 0; j < nodesPerPath; j++)
    {
        double x = baseX + (j % 2) * 15 + random.NextDouble() * 5 - 2.5;
        double y = baseY + (j / 2) * 10 + random.NextDouble() * 5 - 2.5;
        allNodes[i, j] = new FreeNode(document, x, y);
    }
}

// Создание контуров
for (int i = 0; i < pathCount; i++)
{
    paths[i] = new PathConstruction(document);
    
    for (int j = 0; j < nodesPerPath; j++)
    {
        paths[i].AddSegment(allNodes[i, j], allNodes[i, (j + 1) % nodesPerPath]);
    }
    
    // Установка цвета
    int red = (int)(255 * random.NextDouble());
    int green = (int)(255 * random.NextDouble());
    int blue = (int)(255 * random.NextDouble());
    paths[i].Color = (red << 16) | (green << 8) | blue;
    
    // Установка толщины линии
    paths[i].LineWidth = 1 + (int)(random.NextDouble() * 2);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими контурами и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические контуры");

// Создание контура с возможностью динамического обновления
PathConstruction dynamicPath = new PathConstruction(document);

// Создание начальных узлов
int dynamicNodesCount = 6;
FreeNode[] dynamicNodes = new FreeNode[dynamicNodesCount];

for (int i = 0; i < dynamicNodesCount; i++)
{
    double angle = 2 * Math.PI * i / dynamicNodesCount;
    double x = 50 + 20 * Math.Cos(angle);
    double y = 50 + 20 * Math.Sin(angle);
    dynamicNodes[i] = new FreeNode(document, x, y);
    if (i > 0)
    {
        dynamicPath.AddSegment(dynamicNodes[i - 1], dynamicNodes[i]);
    }
}

dynamicPath.AddSegment(dynamicNodes[dynamicNodesCount - 1], dynamicNodes[0]);
dynamicPath.Color = 255; // Красный цвет

// Создание контура, который будет менять свою форму
PathConstruction morphingPath = new PathConstruction(document);

int morphingNodesCount = 8;
FreeNode[] morphingNodes = new FreeNode[morphingNodesCount];

for (int i = 0; i < morphingNodesCount; i++)
{
    double x = 120 + (i % 4) * 15;
    double y = 40 + (i / 4) * 20;
    morphingNodes[i] = new FreeNode(document, x, y);
    if (i > 0)
    {
        morphingPath.AddSegment(morphingNodes[i - 1], morphingNodes[i]);
    }
}

morphingPath.AddSegment(morphingNodes[morphingNodesCount - 1], morphingNodes[0]);
morphingPath.Color = 65280; // Зеленый цвет

// Создание системы контуров с анимацией
int animatedPathCount = 5;
PathConstruction[] animatedPaths = new PathConstruction[animatedPathCount];
FreeNode[,][] animatedNodes = new FreeNode[animatedPathCount, 5][];

for (int i = 0; i < animatedPathCount; i++)
{
    animatedPaths[i] = new PathConstruction(document);
    animatedNodes[i] = new FreeNode[5][];
    
    for (int j = 0; j < 5; j++)
    {
        double baseX = 30 + i * 30;
        double baseY = 100 + j * 15;
        animatedNodes[i][j] = new FreeNode(document, baseX, baseY);
        if (j > 0)
        {
            animatedPaths[i].AddSegment(animatedNodes[i][j - 1], animatedNodes[i][j]);
        }
    }
    
    animatedPaths[i].AddSegment(animatedNodes[i][4], animatedNodes[i][0]);
    animatedPaths[i].Color = 16711680; // Синий цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств контуров
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicPaths(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических контуров");
    
    // Обновление узлов динамического контура
    for (int i = 0; i < dynamicNodesCount; i++)
    {
        double angle = 2 * Math.PI * i / dynamicNodesCount + time * 0.2;
        double x = 50 + 20 * Math.Cos(angle);
        double y = 50 + 20 * Math.Sin(angle);
        dynamicNodes[i].X.Value = x;
        dynamicNodes[i].Y.Value = y;
    }
    
    // Обновление узлов морфирующего контура
    for (int i = 0; i < morphingNodesCount; i++)
    {
        double x = 120 + (i % 4) * 15 + 5 * Math.Sin(time * 0.3 + i);
        double y = 40 + (i / 4) * 20 + 5 * Math.Cos(time * 0.3 + i);
        morphingNodes[i].X.Value = x;
        morphingNodes[i].Y.Value = y;
    }
    
    // Обновление анимированных контуров
    for (int i = 0; i < animatedPathCount; i++)
    {
        for (int j = 0; j < 5; j++)
        {
            double x = 30 + i * 30 + 3 * Math.Sin(time * 0.5 + i + j);
            double y = 100 + j * 15 + 2 * Math.Cos(time * 0.7 + i + j);
            animatedNodes[i][j].X.Value = x;
            animatedNodes[i][j].Y.Value = y;
        }
        
        // Изменение цвета в зависимости от времени
        int red = (int)(255 * (1 + Math.Sin(time * 0.5 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.5 + i + 1)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.5 + i + 2)) / 2);
        animatedPaths[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
```

## Свойства и методы

### Основные свойства:

- `Segments` - Коллекция сегментов контура
- `IsClosed` - Является ли контур замкнутым
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

### Основные методы:

- `AddSegment` - Добавление сегмента к контуру
- `RemoveSegment` - Удаление сегмента из контура
- `InsertSegment` - Вставка сегмента в контур
- `ClearSegments` - Очистка всех сегментов контура
- `GetPoint` - Получение точки на контуре
- `GetTangent` - Получение касательной к контуру

## Заключение

Продвинутое использование класса `PathConstruction` включает в себя создание сложных контуров, параметризованных конструкций, работу с массивами контуров, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами контуров важно учитывать производительность и использовать эффективные алгоритмы для вычисления координат и установления связей между объектами.
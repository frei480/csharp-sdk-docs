# LineConstruction - продвинутые примеры использования

Класс `LineConstruction` представляет линию построения в T-Flex CAD API. Это один из основных классов для создания геометрических конструкций.

## Продвинутые примеры использования

### 1. Создание сложных геометрических конструкций

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сложной геометрической конструкции");

// Создание каркаса сложной конструкции
FreeNode center = new FreeNode(document, 50, 50);
double radius = 30;
int segments = 12;

// Создание радиальных линий
LineConstruction[] radialLines = new LineConstruction[segments];
for (int i = 0; i < segments; i++)
{
    double angle = 2 * Math.PI * i / segments;
    double x = center.X.Value + radius * Math.Cos(angle);
    double y = center.Y.Value + radius * Math.Sin(angle);
    FreeNode endPoint = new FreeNode(document, x, y);
    radialLines[i] = new LineConstruction(document);
    radialLines[i].SetTwoNodes(center, endPoint);
    radialLines[i].Color = 255; // Красный цвет
}

// Создание концентрических окружностей из сегментов линий
double[] radii = { 10, 20, 30 };
LineConstruction[][] concentricCircles = new LineConstruction[radii.Length][];

for (int r = 0; r < radii.Length; r++)
{
    concentricCircles[r] = new LineConstruction[segments];
    FreeNode[] points = new FreeNode[segments];
    
    // Создание точек окружности
    for (int i = 0; i < segments; i++)
    {
        double angle = 2 * Math.PI * i / segments;
        double x = center.X.Value + radii[r] * Math.Cos(angle);
        double y = center.Y.Value + radii[r] * Math.Sin(angle);
        points[i] = new FreeNode(document, x, y);
    }
    
    // Создание сегментов окружности
    for (int i = 0; i < segments; i++)
    {
        concentricCircles[r][i] = new LineConstruction(document);
        concentricCircles[r][i].SetTwoNodes(points[i], points[(i + 1) % segments]);
        concentricCircles[r][i].Color = 65280; // Зеленый цвет
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание параметризованных конструкций

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной конструкции");

// Параметры конструкции
double centerX = 50;
double centerY = 50;
double width = 40;
double height = 30;
double cornerRadius = 5;

// Создание узлов для прямоугольника со скругленными углами
FreeNode[] corners = new FreeNode[4];
corners[0] = new FreeNode(document, centerX - width/2, centerY - height/2); // Левый нижний
corners[1] = new FreeNode(document, centerX + width/2, centerY - height/2); // Правый нижний
corners[2] = new FreeNode(document, centerX + width/2, centerY + height/2); // Правый верхний
corners[3] = new FreeNode(document, centerX - width/2, centerY + height/2); // Левый верхний

// Создание линий со скругленными углами
for (int i = 0; i < 4; i++)
{
    FreeNode startCorner = corners[i];
    FreeNode endCorner = corners[(i + 1) % 4];
    
    // Создание скругления углов
    // Для упрощения используем дуги окружностей
    double startAngle = Math.PI * i / 2;
    double endAngle = Math.PI * (i + 1) / 2;
    
    // Создание точек для дуги
    FreeNode arcCenter = new FreeNode(document, 
        startCorner.X.Value + (i == 0 || i == 3 ? cornerRadius : -cornerRadius),
        startCorner.Y.Value + (i < 2 ? cornerRadius : -cornerRadius));
    
    // Создание дуги (в реальной реализации может потребоваться специальный класс для дуг)
    // Здесь используем приближение дуги сегментами линий
    int arcSegments = 8;
    FreeNode[] arcPoints = new FreeNode[arcSegments + 1];
    
    for (int j = 0; j <= arcSegments; j++)
    {
        double angle = startAngle + (endAngle - startAngle) * j / arcSegments;
        double x = arcCenter.X.Value + cornerRadius * Math.Cos(angle);
        double y = arcCenter.Y.Value + cornerRadius * Math.Sin(angle);
        arcPoints[j] = new FreeNode(document, x, y);
    }
    
    // Создание сегментов дуги
    for (int j = 0; j < arcSegments; j++)
    {
        LineConstruction arcSegment = new LineConstruction(document);
        arcSegment.SetTwoNodes(arcPoints[j], arcPoints[j + 1]);
        arcSegment.Color = 16711680; // Синий цвет
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание конструкций с использованием массивов и циклов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание конструкции с массивами");

// Создание сетки линий
int rows = 10;
int cols = 15;
double spacing = 8.0;
double startX = 10.0;
double startY = 10.0;

// Создание горизонтальных линий
LineConstruction[] horizontalLines = new LineConstruction[rows];
for (int i = 0; i < rows; i++)
{
    double y = startY + i * spacing;
    FreeNode startNode = new FreeNode(document, startX, y);
    FreeNode endNode = new FreeNode(document, startX + (cols - 1) * spacing, y);
    horizontalLines[i] = new LineConstruction(document);
    horizontalLines[i].SetTwoNodes(startNode, endNode);
    horizontalLines[i].Color = 12632256; // Серый цвет
}

// Создание вертикальных линий
LineConstruction[] verticalLines = new LineConstruction[cols];
for (int i = 0; i < cols; i++)
{
    double x = startX + i * spacing;
    FreeNode startNode = new FreeNode(document, x, startY);
    FreeNode endNode = new FreeNode(document, x, startY + (rows - 1) * spacing);
    verticalLines[i] = new LineConstruction(document);
    verticalLines[i].SetTwoNodes(startNode, endNode);
    verticalLines[i].Color = 12632256; // Серый цвет
}

// Создание диагональных линий
LineConstruction[] diagonalLines = new LineConstruction[Math.Min(rows, cols) * 2 - 1];
int diagonalIndex = 0;

// Диагонали слева направо сверху вниз
for (int i = 0; i < rows; i++)
{
    int startCol = 0;
    int startRow = i;
    int endCol = Math.Min(cols - 1, rows - 1 - i);
    int endRow = i + endCol;
    
    FreeNode startNode = new FreeNode(document, 
        startX + startCol * spacing, startY + startRow * spacing);
    FreeNode endNode = new FreeNode(document, 
        startX + endCol * spacing, startY + endRow * spacing);
    
    diagonalLines[diagonalIndex] = new LineConstruction(document);
    diagonalLines[diagonalIndex].SetTwoNodes(startNode, endNode);
    diagonalLines[diagonalIndex].Color = 16776960; // Желтый цвет
    diagonalIndex++;
}

// Диагонали справа налево сверху вниз
for (int i = 1; i < cols; i++)
{
    int startCol = i;
    int startRow = 0;
    int endCol = Math.Min(cols - 1, i + rows - 1);
    int endRow = endCol - i;
    
    FreeNode startNode = new FreeNode(document, 
        startX + startCol * spacing, startY + startRow * spacing);
    FreeNode endNode = new FreeNode(document, 
        startX + endCol * spacing, startY + endRow * spacing);
    
    diagonalLines[diagonalIndex] = new LineConstruction(document);
    diagonalLines[diagonalIndex].SetTwoNodes(startNode, endNode);
    diagonalLines[diagonalIndex].Color = 16776960; // Желтый цвет
    diagonalIndex++;
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция с другими объектами и сложные связи

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция с другими объектами");

// Создание системы взаимосвязанных линий
FreeNode center = new FreeNode(document, 50, 50);
double mainRadius = 40;
int mainSegments = 8;

// Создание основной звезды
FreeNode[] mainPoints = new FreeNode[mainSegments];
LineConstruction[] mainLines = new LineConstruction[mainSegments];

for (int i = 0; i < mainSegments; i++)
{
    double angle = 2 * Math.PI * i / mainSegments;
    double x = center.X.Value + mainRadius * Math.Cos(angle);
    double y = center.Y.Value + mainRadius * Math.Sin(angle);
    mainPoints[i] = new FreeNode(document, x, y);
    
    mainLines[i] = new LineConstruction(document);
    mainLines[i].SetTwoNodes(center, mainPoints[i]);
    mainLines[i].Color = 255; // Красный цвет
}

// Создание внешней оболочки
for (int i = 0; i < mainSegments; i++)
{
    LineConstruction outerLine = new LineConstruction(document);
    outerLine.SetTwoNodes(mainPoints[i], mainPoints[(i + 1) % mainSegments]);
    outerLine.Color = 65280; // Зеленый цвет
}

// Создание внутренней звезды меньшего радиуса
double innerRadius = 20;
FreeNode[] innerPoints = new FreeNode[mainSegments];
LineConstruction[] innerLines = new LineConstruction[mainSegments];

for (int i = 0; i < mainSegments; i++)
{
    double angle = 2 * Math.PI * (i + 0.5) / mainSegments; // Смещение на половину сегмента
    double x = center.X.Value + innerRadius * Math.Cos(angle);
    double y = center.Y.Value + innerRadius * Math.Sin(angle);
    innerPoints[i] = new FreeNode(document, x, y);
    
    innerLines[i] = new LineConstruction(document);
    innerLines[i].SetTwoNodes(center, innerPoints[i]);
    innerLines[i].Color = 16711680; // Синий цвет
}

// Создание связей между внешней и внутренней звездами
for (int i = 0; i < mainSegments; i++)
{
    LineConstruction connectionLine = new LineConstruction(document);
    connectionLine.SetTwoNodes(mainPoints[i], innerPoints[(i + mainSegments/2) % mainSegments]);
    connectionLine.Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством линий

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества линий с минимальными вызовами API
int lineCount = 500;
LineConstruction[] lines = new LineConstruction[lineCount];

// Предварительное создание узлов
FreeNode[] startNodes = new FreeNode[lineCount];
FreeNode[] endNodes = new FreeNode[lineCount];

Random random = new Random();
for (int i = 0; i < lineCount; i++)
{
    // Создание узлов с случайными координатами
    startNodes[i] = new FreeNode(document, 
        random.NextDouble() * 200, 
        random.NextDouble() * 150);
    endNodes[i] = new FreeNode(document, 
        random.NextDouble() * 200, 
        random.NextDouble() * 150);
}

// Создание линий
for (int i = 0; i < lineCount; i++)
{
    lines[i] = new LineConstruction(document);
    lines[i].SetTwoNodes(startNodes[i], endNodes[i]);
    
    // Установка цвета в зависимости от длины линии
    double dx = endNodes[i].X.Value - startNodes[i].X.Value;
    double dy = endNodes[i].Y.Value - startNodes[i].Y.Value;
    double length = Math.Sqrt(dx * dx + dy * dy);
    
    if (length < 20)
        lines[i].Color = 255; // Красный для коротких линий
    else if (length < 50)
        lines[i].Color = 65280; // Зеленый для средних линий
    else
        lines[i].Color = 16711680; // Синий для длинных линий
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими линиями и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические линии");

// Создание линии с возможностью динамического обновления
FreeNode dynamicStart = new FreeNode(document, 30, 30);
FreeNode dynamicEnd = new FreeNode(document, 70, 70);
LineConstruction dynamicLine = new LineConstruction(document);
dynamicLine.SetTwoNodes(dynamicStart, dynamicEnd);
dynamicLine.Color = 255; // Красный цвет

// Создание линии, которая будет менять свой цвет в зависимости от длины
FreeNode colorChangingStart = new FreeNode(document, 20, 80);
FreeNode colorChangingEnd = new FreeNode(document, 80, 20);
LineConstruction colorChangingLine = new LineConstruction(document);
colorChangingLine.SetTwoNodes(colorChangingStart, colorChangingEnd);

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств линий
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicLine(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамической линии");
    
    // Обновление координат конечной точки
    double newX = 70 + 20 * Math.Sin(time * 0.1);
    double newY = 70 + 20 * Math.Cos(time * 0.1);
    dynamicEnd.X.Value = newX;
    dynamicEnd.Y.Value = newY;
    
    // Обновление цвета в зависимости от длины
    double dx = dynamicEnd.X.Value - dynamicStart.X.Value;
    double dy = dynamicEnd.Y.Value - dynamicStart.Y.Value;
    double length = Math.Sqrt(dx * dx + dy * dy);
    
    // Интерполяция цвета от зеленого к красному в зависимости от длины
    int red = (int)(255 * Math.Min(1.0, length / 100.0));
    int green = (int)(255 * Math.Max(0.0, 1.0 - length / 100.0));
    dynamicLine.Color = (red << 16) | (green << 8);
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
```

## Свойства и методы

### Основные свойства:

- `SubType` - Подтип линии построения
- `GeometryType` - Тип геометрии линии построения
- `Param` - Значение параметра линии построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым

### Основные методы:

- `SetTwoNodes` - Установка двух узлов для определения линии
- `SetPointAndAngle` - Установка точки и угла наклона
- `SetTwoPoints` - Установка двух точек для определения линии
- `SetPointAndDirection` - Установка точки и направления

## Заключение

Продвинутое использование класса `LineConstruction` включает в себя создание сложных геометрических конструкций, параметризованных объектов, работу с массивами линий, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами линий важно учитывать производительность и использовать эффективные алгоритмы для вычисления координат и установления связей между объектами.
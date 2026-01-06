# EllipseConstruction - продвинутые примеры использования

Класс `EllipseConstruction` представляет эллипс построения в T-Flex CAD API. Этот класс предоставляет возможности для создания эллипсов различными способами.

## Продвинутые примеры использования

### 1. Создание системы вложенных эллипсов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание системы вложенных эллипсов");

// Создание центра системы
FreeNode center = new FreeNode(document, 50, 50);

// Создание вложенных эллипсов с разными параметрами
int ellipseCount = 8;
EllipseConstruction[] ellipses = new EllipseConstruction[ellipseCount];

for (int i = 0; i < ellipseCount; i++)
{
    ellipses[i] = new EllipseConstruction(document);
    
    // Вычисление параметров эллипса
    double majorRadius = 5 + i * 3;
    double minorRadius = 3 + i * 2;
    
    // Создание узлов для определения эллипса
    FreeNode majorNode = new FreeNode(document, center.X.Value + majorRadius, center.Y.Value);
    FreeNode minorNode = new FreeNode(document, center.X.Value, center.Y.Value + minorRadius);
    
    // Установка эллипса через центр и два узла
    ellipses[i].SetCenterAndTwoNodes(center, majorNode, minorNode);
    
    // Установка цвета с градиентом
    int intensity = (int)(255 * (double)i / (ellipseCount - 1));
    ellipses[i].Color = (intensity << 16) | ((255 - intensity) << 8) | 128;
    
    // Установка толщины линии
    ellipses[i].LineWidth = 1 + i / 3;
}

// Создание радиальных линий для деления эллипсов
int radialLinesCount = 16;
LineConstruction[] radialLines = new LineConstruction[radialLinesCount];

for (int i = 0; i < radialLinesCount; i++)
{
    double angle = 2 * Math.PI * i / radialLinesCount;
    double maxLength = 40;
    double endX = center.X.Value + maxLength * Math.Cos(angle);
    double endY = center.Y.Value + maxLength * Math.Sin(angle);
    
    FreeNode endPoint = new FreeNode(document, endX, endY);
    radialLines[i] = new LineConstruction(document);
    radialLines[i].SetTwoNodes(center, endPoint);
    radialLines[i].Color = 12632256; // Серый цвет
    radialLines[i].Style = LineStyle.Dash; // Пунктирная линия
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание эллипсов с геометрическими расчетами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание эллипсов с геометрическими расчетами");

// Создание эллипса, вписанного в прямоугольник
double rectWidth = 60;
double rectHeight = 40;
FreeNode rectCenter = new FreeNode(document, 50, 50);

// Создание узлов прямоугольника
FreeNode[] rectCorners = new FreeNode[4];
rectCorners[0] = new FreeNode(document, rectCenter.X.Value - rectWidth/2, rectCenter.Y.Value - rectHeight/2);
rectCorners[1] = new FreeNode(document, rectCenter.X.Value + rectWidth/2, rectCenter.Y.Value - rectHeight/2);
rectCorners[2] = new FreeNode(document, rectCenter.X.Value + rectWidth/2, rectCenter.Y.Value + rectHeight/2);
rectCorners[3] = new FreeNode(document, rectCenter.X.Value - rectWidth/2, rectCenter.Y.Value + rectHeight/2);

// Создание сторон прямоугольника
LineConstruction[] rectSides = new LineConstruction[4];
for (int i = 0; i < 4; i++)
{
    rectSides[i] = new LineConstruction(document);
    rectSides[i].SetTwoNodes(rectCorners[i], rectCorners[(i + 1) % 4]);
    rectSides[i].Color = 12632256; // Серый цвет
}

// Создание вписанного эллипса
EllipseConstruction inscribedEllipse = new EllipseConstruction(document);
FreeNode majorNode = new FreeNode(document, rectCenter.X.Value + rectWidth/2, rectCenter.Y.Value);
FreeNode minorNode = new FreeNode(document, rectCenter.X.Value, rectCenter.Y.Value + rectHeight/2);
inscribedEllipse.SetCenterAndTwoNodes(rectCenter, majorNode, minorNode);
inscribedEllipse.Color = 255; // Красный цвет

// Создание описанного эллипса
double circumscribedMajor = Math.Sqrt(rectWidth * rectWidth + rectHeight * rectHeight) / 2;
double circumscribedMinor = circumscribedMajor;
EllipseConstruction circumscribedEllipse = new EllipseConstruction(document);
FreeNode circumscribedMajorNode = new FreeNode(document, rectCenter.X.Value + circumscribedMajor, rectCenter.Y.Value);
FreeNode circumscribedMinorNode = new FreeNode(document, rectCenter.X.Value, rectCenter.Y.Value + circumscribedMinor);
circumscribedEllipse.SetCenterAndTwoNodes(rectCenter, circumscribedMajorNode, circumscribedMinorNode);
circumscribedEllipse.Color = 65280; // Зеленый цвет

// Создание фокусов эллипса
// Для вписанного эллипса
double focusDistance = Math.Sqrt((rectWidth/2) * (rectWidth/2) - (rectHeight/2) * (rectHeight/2));
FreeNode[] foci = new FreeNode[2];
if (focusDistance > 0)
{
    foci[0] = new FreeNode(document, rectCenter.X.Value - focusDistance, rectCenter.Y.Value);
    foci[1] = new FreeNode(document, rectCenter.X.Value + focusDistance, rectCenter.Y.Value);
    
    // Создание точек фокусов
    CircleConstruction[] focusCircles = new CircleConstruction[2];
    for (int i = 0; i < 2; i++)
    {
        focusCircles[i] = new CircleConstruction(document);
        focusCircles[i].SetCenterAndRadius(foci[i], 1);
        focusCircles[i].Color = 16711680; // Синий цвет
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание эллипсов с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы эллипсов");

// Параметры системы эллипсов
int rows = 4;
int cols = 5;
double spacingX = 30.0;
double spacingY = 25.0;
double baseMajor = 8.0;
double baseMinor = 5.0;
double startX = 25.0;
double startY = 25.0;

// Создание двумерного массива эллипсов
EllipseConstruction[,] ellipseGrid = new EllipseConstruction[rows, cols];

for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols; j++)
    {
        // Вычисление центра эллипса
        double centerX = startX + j * spacingX;
        double centerY = startY + i * spacingY;
        FreeNode center = new FreeNode(document, centerX, centerY);
        
        // Вычисление параметров в зависимости от позиции
        double majorRadius = baseMajor + (i + j) * 0.5;
        double minorRadius = baseMinor + (i - j) * 0.3;
        
        // Создание узлов для определения эллипса
        FreeNode majorNode = new FreeNode(document, centerX + majorRadius, centerY);
        FreeNode minorNode = new FreeNode(document, centerX, centerY + minorRadius);
        
        // Создание эллипса
        ellipseGrid[i, j] = new EllipseConstruction(document);
        ellipseGrid[i, j].SetCenterAndTwoNodes(center, majorNode, minorNode);
        
        // Установка цвета с градиентом
        int red = (int)(255 * (double)i / (rows - 1));
        int green = (int)(255 * (double)j / (cols - 1));
        int blue = 255 - (red + green) / 2;
        ellipseGrid[i, j].Color = (red << 16) | (green << 8) | blue;
        
        // Установка толщины линии
        ellipseGrid[i, j].LineWidth = 1 + (i + j) / 4;
    }
}

// Создание соединительных линий между центрами эллипсов
for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols - 1; j++)
    {
        LineConstruction line = new LineConstruction(document);
        FreeNode startCenter = new FreeNode(document, 
            startX + j * spacingX, startY + i * spacingY);
        FreeNode endCenter = new FreeNode(document, 
            startX + (j + 1) * spacingX, startY + i * spacingY);
        line.SetTwoNodes(startCenter, endCenter);
        line.Color = 12632256; // Серый цвет
        line.Style = LineStyle.Dot; // Точечная линия
    }
}

for (int i = 0; i < rows - 1; i++)
{
    for (int j = 0; j < cols; j++)
    {
        LineConstruction line = new LineConstruction(document);
        FreeNode startCenter = new FreeNode(document, 
            startX + j * spacingX, startY + i * spacingY);
        FreeNode endCenter = new FreeNode(document, 
            startX + j * spacingX, startY + (i + 1) * spacingY);
        line.SetTwoNodes(startCenter, endCenter);
        line.Color = 12632256; // Серый цвет
        line.Style = LineStyle.Dot; // Точечная линия
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция эллипсов с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция эллипсов с другими объектами");

// Создание системы эллипсов и линий
FreeNode center = new FreeNode(document, 50, 50);
double majorRadius = 30;
double minorRadius = 20;

// Создание основного эллипса
EllipseConstruction mainEllipse = new EllipseConstruction(document);
FreeNode majorNode = new FreeNode(document, center.X.Value + majorRadius, center.Y.Value);
FreeNode minorNode = new FreeNode(document, center.X.Value, center.Y.Value + minorRadius);
mainEllipse.SetCenterAndTwoNodes(center, majorNode, minorNode);
mainEllipse.Color = 255; // Красный цвет

// Создание вписанных эллипсов
int inscribedCount = 6;
EllipseConstruction[] inscribedEllipses = new EllipseConstruction[inscribedCount];

for (int i = 0; i < inscribedCount; i++)
{
    double angle = 2 * Math.PI * i / inscribedCount;
    double scale = 0.6;
    double inscribedMajor = majorRadius * scale;
    double inscribedMinor = minorRadius * scale;
    double inscribedCenterX = center.X.Value + (majorRadius - inscribedMajor) * Math.Cos(angle);
    double inscribedCenterY = center.Y.Value + (minorRadius - inscribedMinor) * Math.Sin(angle);
    
    FreeNode inscribedCenter = new FreeNode(document, inscribedCenterX, inscribedCenterY);
    FreeNode inscribedMajorNode = new FreeNode(document, 
        inscribedCenterX + inscribedMajor, inscribedCenterY);
    FreeNode inscribedMinorNode = new FreeNode(document, 
        inscribedCenterX, inscribedCenterY + inscribedMinor);
    
    inscribedEllipses[i] = new EllipseConstruction(document);
    inscribedEllipses[i].SetCenterAndTwoNodes(inscribedCenter, inscribedMajorNode, inscribedMinorNode);
    inscribedEllipses[i].Color = 65280; // Зеленый цвет
}

// Создание описанных эллипсов
int circumscribedCount = 6;
EllipseConstruction[] circumscribedEllipses = new EllipseConstruction[circumscribedCount];

for (int i = 0; i < circumscribedCount; i++)
{
    double angle = 2 * Math.PI * (i + 0.5) / circumscribedCount;
    double scale = 1.4;
    double circumscribedMajor = majorRadius * scale;
    double circumscribedMinor = minorRadius * scale;
    double circumscribedCenterX = center.X.Value + circumscribedMajor * Math.Cos(angle);
    double circumscribedCenterY = center.Y.Value + circumscribedMinor * Math.Sin(angle);
    
    FreeNode circumscribedCenter = new FreeNode(document, circumscribedCenterX, circumscribedCenterY);
    FreeNode circumscribedMajorNode = new FreeNode(document, 
        circumscribedCenterX + circumscribedMajor, circumscribedCenterY);
    FreeNode circumscribedMinorNode = new FreeNode(document, 
        circumscribedCenterX, circumscribedCenterY + circumscribedMinor);
    
    circumscribedEllipses[i] = new EllipseConstruction(document);
    circumscribedEllipses[i].SetCenterAndTwoNodes(circumscribedCenter, circumscribedMajorNode, circumscribedMinorNode);
    circumscribedEllipses[i].Color = 16711680; // Синий цвет
}

// Создание касательных линий
int tangentLinesCount = 12;
LineConstruction[] tangentLines = new LineConstruction[tangentLinesCount];

for (int i = 0; i < tangentLinesCount; i++)
{
    double angle = 2 * Math.PI * i / tangentLinesCount;
    // Вычисление точки на эллипсе (приблизительно)
    double x = center.X.Value + majorRadius * Math.Cos(angle);
    double y = center.Y.Value + minorRadius * Math.Sin(angle);
    double tangentX = center.X.Value + majorRadius * 1.5 * Math.Cos(angle);
    double tangentY = center.Y.Value + minorRadius * 1.5 * Math.Sin(angle);
    
    FreeNode startPoint = new FreeNode(document, x, y);
    FreeNode endPoint = new FreeNode(document, tangentX, tangentY);
    tangentLines[i] = new LineConstruction(document);
    tangentLines[i].SetTwoNodes(startPoint, endPoint);
    tangentLines[i].Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством эллипсов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества эллипсов с минимальными вызовами API
int ellipseCount = 200;
EllipseConstruction[] ellipses = new EllipseConstruction[ellipseCount];

// Предварительное создание узлов
FreeNode[] centers = new FreeNode[ellipseCount];
FreeNode[] majorNodes = new FreeNode[ellipseCount];
FreeNode[] minorNodes = new FreeNode[ellipseCount];

Random random = new Random();
for (int i = 0; i < ellipseCount; i++)
{
    // Создание узлов с случайными координатами
    double centerX = 20 + random.NextDouble() * 160;
    double centerY = 20 + random.NextDouble() * 110;
    centers[i] = new FreeNode(document, centerX, centerY);
    
    double majorRadius = 3 + random.NextDouble() * 7;
    double minorRadius = 2 + random.NextDouble() * 5;
    majorNodes[i] = new FreeNode(document, centerX + majorRadius, centerY);
    minorNodes[i] = new FreeNode(document, centerX, centerY + minorRadius);
}

// Создание эллипсов
for (int i = 0; i < ellipseCount; i++)
{
    ellipses[i] = new EllipseConstruction(document);
    ellipses[i].SetCenterAndTwoNodes(centers[i], majorNodes[i], minorNodes[i]);
    
    // Установка цвета в зависимости от параметров
    int red = (int)(255 * random.NextDouble());
    int green = (int)(255 * random.NextDouble());
    int blue = (int)(255 * random.NextDouble());
    ellipses[i].Color = (red << 16) | (green << 8) | blue;
    
    // Установка толщины линии
    ellipses[i].LineWidth = 1 + (int)(random.NextDouble() * 3);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими эллипсами и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические эллипсы");

// Создание эллипса с возможностью динамического обновления
FreeNode dynamicCenter = new FreeNode(document, 50, 50);
FreeNode dynamicMajor = new FreeNode(document, 80, 50);
FreeNode dynamicMinor = new FreeNode(document, 50, 70);
EllipseConstruction dynamicEllipse = new EllipseConstruction(document);
dynamicEllipse.SetCenterAndTwoNodes(dynamicCenter, dynamicMajor, dynamicMinor);
dynamicEllipse.Color = 255; // Красный цвет

// Создание эллипса, который будет менять свои параметры
FreeNode pulsatingCenter = new FreeNode(document, 120, 100);
EllipseConstruction pulsatingEllipse = new EllipseConstruction(document);
FreeNode pulsatingMajor = new FreeNode(document, 150, 100);
FreeNode pulsatingMinor = new FreeNode(document, 120, 120);
pulsatingEllipse.SetCenterAndTwoNodes(pulsatingCenter, pulsatingMajor, pulsatingMinor);
pulsatingEllipse.Color = 65280; // Зеленый цвет

// Создание системы эллипсов с анимацией
int animatedCount = 6;
FreeNode[] animatedCenters = new FreeNode[animatedCount];
FreeNode[] animatedMajorNodes = new FreeNode[animatedCount];
FreeNode[] animatedMinorNodes = new FreeNode[animatedCount];
EllipseConstruction[] animatedEllipses = new EllipseConstruction[animatedCount];

for (int i = 0; i < animatedCount; i++)
{
    double angle = 2 * Math.PI * i / animatedCount;
    double centerX = 170 + 30 * Math.Cos(angle);
    double centerY = 50 + 30 * Math.Sin(angle);
    animatedCenters[i] = new FreeNode(document, centerX, centerY);
    
    double majorX = centerX + 10;
    double minorY = centerY + 8;
    animatedMajorNodes[i] = new FreeNode(document, majorX, centerY);
    animatedMinorNodes[i] = new FreeNode(document, centerX, minorY);
    
    animatedEllipses[i] = new EllipseConstruction(document);
    animatedEllipses[i].SetCenterAndTwoNodes(animatedCenters[i], animatedMajorNodes[i], animatedMinorNodes[i]);
    animatedEllipses[i].Color = 16711680; // Синий цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств эллипсов
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicEllipses(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических эллипсов");
    
    // Обновление позиции центра
    double newX = 50 + 20 * Math.Sin(time * 0.2);
    double newY = 50 + 20 * Math.Cos(time * 0.2);
    dynamicCenter.X.Value = newX;
    dynamicCenter.Y.Value = newY;
    
    // Обновление параметров пульсирующего эллипса
    double majorScale = 1 + 0.3 * Math.Sin(time * 0.5);
    double minorScale = 1 + 0.3 * Math.Cos(time * 0.5);
    dynamicMajor.X.Value = dynamicCenter.X.Value + 30 * majorScale;
    dynamicMinor.Y.Value = dynamicCenter.Y.Value + 20 * minorScale;
    
    // Обновление анимированных эллипсов
    for (int i = 0; i < animatedCount; i++)
    {
        double angle = 2 * Math.PI * i / animatedCount + time * 0.3;
        double centerX = 170 + 30 * Math.Cos(angle);
        double centerY = 50 + 30 * Math.Sin(angle);
        animatedCenters[i].X.Value = centerX;
        animatedCenters[i].Y.Value = centerY;
        
        double majorX = centerX + 10 + 5 * Math.Sin(time * 0.7 + i);
        double minorY = centerY + 8 + 4 * Math.Cos(time * 0.7 + i);
        animatedMajorNodes[i].X.Value = majorX;
        animatedMinorNodes[i].Y.Value = minorY;
        
        // Изменение цвета в зависимости от позиции
        int red = (int)(255 * (1 + Math.Sin(angle)) / 2);
        int green = (int)(255 * (1 + Math.Cos(angle * 2)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(angle * 3)) / 2);
        animatedEllipses[i].Color = (red << 16) | (green << 8) | blue;
    }
    
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
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

### Основные методы:

- `SetCenterAndTwoNodes` - Установка эллипса через центр и два узла
- `SetCenterAndTwoPoints` - Установка эллипса через центр и две точки
- `SetFivePoints` - Установка эллипса по пяти точкам
- `SetFiveNodes` - Установка эллипса по пяти узлам

## Заключение

Продвинутое использование класса `EllipseConstruction` включает в себя создание сложных систем эллипсов, параметризованных конструкций, работу с массивами эллипсов, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами эллипсов важно учитывать производительность и использовать эффективные алгоритмы для вычисления координат и установления связей между объектами.
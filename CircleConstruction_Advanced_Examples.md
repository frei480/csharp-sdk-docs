# CircleConstruction - продвинутые примеры использования

Класс `CircleConstruction` представляет окружность построения в T-Flex CAD API. Это один из основных классов для создания геометрических конструкций.

## Продвинутые примеры использования

### 1. Создание системы концентрических окружностей

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание системы концентрических окружностей");

// Создание центра системы
FreeNode center = new FreeNode(document, 50, 50);

// Создание концентрических окружностей с разными радиусами
double[] radii = { 5, 10, 15, 20, 25, 30 };
int[] colors = { 255, 65280, 16711680, 16776960, 65535, 16711935 };

CircleConstruction[] circles = new CircleConstruction[radii.Length];

for (int i = 0; i < radii.Length; i++)
{
    circles[i] = new CircleConstruction(document);
    circles[i].SetCenterAndRadius(center, radii[i]);
    circles[i].Color = colors[i];
    
    // Дополнительные свойства
    circles[i].LineWidth = (i % 2 == 0) ? 1 : 2; // Разная толщина линий
}

// Создание радиальных линий для деления окружностей
int radialLinesCount = 12;
LineConstruction[] radialLines = new LineConstruction[radialLinesCount];

for (int i = 0; i < radialLinesCount; i++)
{
    double angle = 2 * Math.PI * i / radialLinesCount;
    double maxLength = radii[radii.Length - 1] + 10;
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

### 2. Создание окружностей по трем точкам с геометрическими расчетами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание окружностей по трем точкам");

// Создание точек для определения окружности
FreeNode point1 = new FreeNode(document, 30, 30);
FreeNode point2 = new FreeNode(document, 70, 30);
FreeNode point3 = new FreeNode(document, 50, 70);

// Создание окружности по трем точкам
CircleConstruction circle = new CircleConstruction(document);
circle.SetThreePoints(point1, point2, point3);
circle.Color = 255; // Красный цвет

// Создание вспомогательных линий между точками
LineConstruction[] helperLines = new LineConstruction[3];
helperLines[0] = new LineConstruction(document);
helperLines[0].SetTwoNodes(point1, point2);
helperLines[0].Color = 12632256; // Серый цвет
helperLines[0].Style = LineStyle.Dash;

helperLines[1] = new LineConstruction(document);
helperLines[1].SetTwoNodes(point2, point3);
helperLines[1].Color = 12632256; // Серый цвет
helperLines[1].Style = LineStyle.Dash;

helperLines[2] = new LineConstruction(document);
helperLines[2].SetTwoNodes(point3, point1);
helperLines[2].Color = 12632256; // Серый цвет
helperLines[2].Style = LineStyle.Dash;

// Создание точек на окружности для демонстрации
int pointsOnCircle = 8;
FreeNode[] circlePoints = new FreeNode[pointsOnCircle];

for (int i = 0; i < pointsOnCircle; i++)
{
    // В реальной реализации здесь потребуется вычисление точек на окружности
    // Для упрощения примера создаем точки вручную
    double angle = 2 * Math.PI * i / pointsOnCircle;
    // Предполагаем, что центр окружности в точке (50, 50) и радиус 20
    double centerX = 50;
    double centerY = 50;
    double radius = 20;
    double x = centerX + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    circlePoints[i] = new FreeNode(document, x, y);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание окружностей с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы окружностей");

// Параметры системы окружностей
int rows = 5;
int cols = 6;
double spacing = 20.0;
double baseRadius = 5.0;
double startX = 20.0;
double startY = 20.0;

// Создание двумерного массива окружностей
CircleConstruction[,] circleGrid = new CircleConstruction[rows, cols];

for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols; j++)
    {
        // Вычисление центра окружности
        double centerX = startX + j * spacing;
        double centerY = startY + i * spacing;
        FreeNode center = new FreeNode(document, centerX, centerY);
        
        // Вычисление радиуса в зависимости от позиции
        double radius = baseRadius + (i + j) * 0.5;
        
        // Создание окружности
        circleGrid[i, j] = new CircleConstruction(document);
        circleGrid[i, j].SetCenterAndRadius(center, radius);
        
        // Установка цвета в зависимости от позиции
        int red = (int)(255 * (double)i / (rows - 1));
        int green = (int)(255 * (double)j / (cols - 1));
        int blue = 255 - (red + green) / 2;
        circleGrid[i, j].Color = (red << 16) | (green << 8) | blue;
        
        // Установка толщины линии в зависимости от радиуса
        circleGrid[i, j].LineWidth = (int)(1 + radius / 5);
    }
}

// Создание соединительных линий между центрами окружностей
for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols - 1; j++)
    {
        LineConstruction line = new LineConstruction(document);
        // Получение центров окружностей (в реальной реализации может потребоваться хранить ссылки на узлы)
        FreeNode startCenter = new FreeNode(document, 
            startX + j * spacing, startY + i * spacing);
        FreeNode endCenter = new FreeNode(document, 
            startX + (j + 1) * spacing, startY + i * spacing);
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
            startX + j * spacing, startY + i * spacing);
        FreeNode endCenter = new FreeNode(document, 
            startX + j * spacing, startY + (i + 1) * spacing);
        line.SetTwoNodes(startCenter, endCenter);
        line.Color = 12632256; // Серый цвет
        line.Style = LineStyle.Dot; // Точечная линия
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция окружностей с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция окружностей с другими объектами");

// Создание системы окружностей и линий
FreeNode center = new FreeNode(document, 50, 50);
double mainRadius = 30;

// Создание основной окружности
CircleConstruction mainCircle = new CircleConstruction(document);
mainCircle.SetCenterAndRadius(center, mainRadius);
mainCircle.Color = 255; // Красный цвет

// Создание вписанных окружностей
int inscribedCount = 6;
CircleConstruction[] inscribedCircles = new CircleConstruction[inscribedCount];

for (int i = 0; i < inscribedCount; i++)
{
    double angle = 2 * Math.PI * i / inscribedCount;
    double inscribedRadius = mainRadius / 3;
    double inscribedCenterX = center.X.Value + (mainRadius - inscribedRadius) * Math.Cos(angle);
    double inscribedCenterY = center.Y.Value + (mainRadius - inscribedRadius) * Math.Sin(angle);
    
    FreeNode inscribedCenter = new FreeNode(document, inscribedCenterX, inscribedCenterY);
    inscribedCircles[i] = new CircleConstruction(document);
    inscribedCircles[i].SetCenterAndRadius(inscribedCenter, inscribedRadius);
    inscribedCircles[i].Color = 65280; // Зеленый цвет
}

// Создание описанных окружностей
int circumscribedCount = 6;
CircleConstruction[] circumscribedCircles = new CircleConstruction[circumscribedCount];

for (int i = 0; i < circumscribedCount; i++)
{
    double angle = 2 * Math.PI * (i + 0.5) / circumscribedCount;
    double circumscribedRadius = mainRadius * 1.5;
    double circumscribedCenterX = center.X.Value + circumscribedRadius * Math.Cos(angle);
    double circumscribedCenterY = center.Y.Value + circumscribedRadius * Math.Sin(angle);
    
    FreeNode circumscribedCenter = new FreeNode(document, circumscribedCenterX, circumscribedCenterY);
    circumscribedCircles[i] = new CircleConstruction(document);
    circumscribedCircles[i].SetCenterAndRadius(circumscribedCenter, mainRadius);
    circumscribedCircles[i].Color = 16711680; // Синий цвет
}

// Создание касательных линий
int tangentLinesCount = 12;
LineConstruction[] tangentLines = new LineConstruction[tangentLinesCount];

for (int i = 0; i < tangentLinesCount; i++)
{
    double angle = 2 * Math.PI * i / tangentLinesCount;
    double startX = center.X.Value + mainRadius * Math.Cos(angle);
    double startY = center.Y.Value + mainRadius * Math.Sin(angle);
    double endX = center.X.Value + mainRadius * 2 * Math.Cos(angle);
    double endY = center.Y.Value + mainRadius * 2 * Math.Sin(angle);
    
    FreeNode startPoint = new FreeNode(document, startX, startY);
    FreeNode endPoint = new FreeNode(document, endX, endY);
    tangentLines[i] = new LineConstruction(document);
    tangentLines[i].SetTwoNodes(startPoint, endPoint);
    tangentLines[i].Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством окружностей

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества окружностей с минимальными вызовами API
int circleCount = 300;
CircleConstruction[] circles = new CircleConstruction[circleCount];

// Предварительное создание узлов
FreeNode[] centers = new FreeNode[circleCount];
double[] radii = new double[circleCount];

Random random = new Random();
for (int i = 0; i < circleCount; i++)
{
    // Создание узлов с случайными координатами
    centers[i] = new FreeNode(document, 
        20 + random.NextDouble() * 160, 
        20 + random.NextDouble() * 110);
    radii[i] = 2 + random.NextDouble() * 8;
}

// Создание окружностей
for (int i = 0; i < circleCount; i++)
{
    circles[i] = new CircleConstruction(document);
    circles[i].SetCenterAndRadius(centers[i], radii[i]);
    
    // Установка цвета в зависимости от радиуса
    int intensity = (int)(255 * (radii[i] - 2) / 8);
    circles[i].Color = (intensity << 16) | (intensity << 8) | (255 - intensity);
    
    // Установка толщины линии в зависимости от радиуса
    circles[i].LineWidth = (int)(1 + radii[i] / 4);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими окружностями и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические окружности");

// Создание окружности с возможностью динамического обновления
FreeNode dynamicCenter = new FreeNode(document, 50, 50);
CircleConstruction dynamicCircle = new CircleConstruction(document);
dynamicCircle.SetCenterAndRadius(dynamicCenter, 20);
dynamicCircle.Color = 255; // Красный цвет

// Создание окружности, которая будет менять свой радиус
FreeNode pulsatingCenter = new FreeNode(document, 100, 100);
CircleConstruction pulsatingCircle = new CircleConstruction(document);
pulsatingCircle.SetCenterAndRadius(pulsatingCenter, 15);
pulsatingCircle.Color = 65280; // Зеленый цвет

// Создание системы окружностей с анимацией
int animatedCount = 8;
FreeNode[] animatedCenters = new FreeNode[animatedCount];
CircleConstruction[] animatedCircles = new CircleConstruction[animatedCount];

for (int i = 0; i < animatedCount; i++)
{
    double angle = 2 * Math.PI * i / animatedCount;
    double centerX = 150 + 30 * Math.Cos(angle);
    double centerY = 50 + 30 * Math.Sin(angle);
    animatedCenters[i] = new FreeNode(document, centerX, centerY);
    
    animatedCircles[i] = new CircleConstruction(document);
    animatedCircles[i].SetCenterAndRadius(animatedCenters[i], 5);
    animatedCircles[i].Color = 16711680; // Синий цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств окружностей
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicCircles(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических окружностей");
    
    // Обновление позиции центра
    double newX = 50 + 20 * Math.Sin(time * 0.2);
    double newY = 50 + 20 * Math.Cos(time * 0.2);
    dynamicCenter.X.Value = newX;
    dynamicCenter.Y.Value = newY;
    
    // Обновление радиуса пульсирующей окружности
    double newRadius = 15 + 10 * Math.Sin(time * 0.5);
    pulsatingCircle.SetCenterAndRadius(pulsatingCenter, Math.Abs(newRadius));
    
    // Обновление анимированных окружностей
    for (int i = 0; i < animatedCount; i++)
    {
        double angle = 2 * Math.PI * i / animatedCount + time * 0.3;
        double centerX = 150 + 30 * Math.Cos(angle);
        double centerY = 50 + 30 * Math.Sin(angle);
        animatedCenters[i].X.Value = centerX;
        animatedCenters[i].Y.Value = centerY;
        
        // Изменение цвета в зависимости от позиции
        int red = (int)(255 * (1 + Math.Sin(angle)) / 2);
        int green = (int)(255 * (1 + Math.Cos(angle * 2)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(angle * 3)) / 2);
        animatedCircles[i].Color = (red << 16) | (green << 8) | blue;
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

- `SetCenterAndRadius` - Установка центра и радиуса окружности
- `SetCenterAndDiameter` - Установка центра и диаметра окружности
- `SetThreePoints` - Установка окружности по трем точкам
- `SetTwoPoints` - Установка окружности по двум точкам (диаметр)

## Заключение

Продвинутое использование класса `CircleConstruction` включает в себя создание сложных систем окружностей, параметризованных конструкций, работу с массивами окружностей, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами окружностей важно учитывать производительность и использовать эффективные алгоритмы для вычисления координат и установления связей между объектами.
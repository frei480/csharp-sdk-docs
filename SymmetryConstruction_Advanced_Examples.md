# SymmetryConstruction - продвинутые примеры использования

Класс `SymmetryConstruction` представляет линию построения, симметричную относительно оси в T-Flex CAD API. Этот класс предоставляет возможности для создания симметричных копий объектов.

## Продвинутые примеры использования

### 1. Создание сложных симметричных конструкций

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сложных симметричных конструкций");

// Создание исходного сложного объекта (звезды с контуром)
PathConstruction sourceStar = new PathConstruction(document);

int starPoints = 8;
double outerRadius = 20;
double innerRadius = 10;
double centerX = 50;
double centerY = 50;

FreeNode[] starNodes = new FreeNode[starPoints * 2];

for (int i = 0; i < starPoints * 2; i++)
{
    double radius = (i % 2 == 0) ? outerRadius : innerRadius;
    double angle = 2 * Math.PI * i / (starPoints * 2) - Math.PI / 2;
    double x = centerX + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    starNodes[i] = new FreeNode(document, x, y);
}

for (int i = 0; i < starPoints * 2; i++)
{
    sourceStar.AddSegment(starNodes[i], starNodes[(i + 1) % (starPoints * 2)]);
}

sourceStar.Color = 255; // Красный цвет

// Создание множественных симметрий
int symmetryCount = 4;
SymmetryConstruction[] starSymmetries = new SymmetryConstruction[symmetryCount];
LineConstruction[] symmetryAxes = new LineConstruction[symmetryCount];

for (int i = 0; i < symmetryCount; i++)
{
    // Создание оси симметрии
    double angle = Math.PI * i / symmetryCount;
    double axisStartX = centerX - 30 * Math.Cos(angle);
    double axisStartY = centerY - 30 * Math.Sin(angle);
    double axisEndX = centerX + 30 * Math.Cos(angle);
    double axisEndY = centerY + 30 * Math.Sin(angle);
    
    FreeNode axisStart = new FreeNode(document, axisStartX, axisStartY);
    FreeNode axisEnd = new FreeNode(document, axisEndX, axisEndY);
    symmetryAxes[i] = new LineConstruction(document);
    symmetryAxes[i].SetTwoNodes(axisStart, axisEnd);
    symmetryAxes[i].Color = 12632256; // Серый цвет
    symmetryAxes[i].Style = LineStyle.Dash; // Пунктирная линия
    
    // Создание симметрии
    starSymmetries[i] = new SymmetryConstruction(document);
    starSymmetries[i].Source = sourceStar;
    starSymmetries[i].Axis = symmetryAxes[i];
    
    // Установка цвета с градиентом
    int red = (int)(255 * (1 + Math.Cos(2 * Math.PI * i / symmetryCount)) / 2);
    int green = (int)(255 * (1 + Math.Cos(2 * Math.PI * i / symmetryCount + 2 * Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Cos(2 * Math.PI * i / symmetryCount + 4 * Math.PI / 3)) / 2);
    starSymmetries[i].Color = (red << 16) | (green << 8) | blue;
}

// Создание симметрий с различными углами
int angleSymmetryCount = 6;
SymmetryConstruction[] angleSymmetries = new SymmetryConstruction[angleSymmetryCount];

for (int i = 0; i < angleSymmetryCount; i++)
{
    angleSymmetries[i] = new SymmetryConstruction(document);
    angleSymmetries[i].Source = sourceStar;
    
    // Создание оси симметрии под разными углами
    double angle = 2 * Math.PI * i / angleSymmetryCount;
    FreeNode axisStart = new FreeNode(document, centerX - 40 * Math.Cos(angle), centerY - 40 * Math.Sin(angle));
    FreeNode axisEnd = new FreeNode(document, centerX + 40 * Math.Cos(angle), centerY + 40 * Math.Sin(angle));
    LineConstruction axis = new LineConstruction(document);
    axis.SetTwoNodes(axisStart, axisEnd);
    axis.Color = 12632256; // Серый цвет
    axis.Style = LineStyle.DashDot; // Штрих-пунктирная линия
    
    angleSymmetries[i].Axis = axis;
    
    // Установка цвета
    int intensity = (int)(255 * (double)i / (angleSymmetryCount - 1));
    angleSymmetries[i].Color = (intensity << 16) | ((255 - intensity) << 8) | 128;
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание симметрий с геометрическими расчетами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание симметрий с геометрическими расчетами");

// Создание исходного объекта (сплайна)
SplineConstruction sourceSpline = new SplineConstruction(document);

// Создание точек сплайна в форме волны
double startX = 30;
double startY = 50;
int splinePoints = 15;
double amplitude = 15;
double wavelength = 5;

for (int i = 0; i <= splinePoints; i++)
{
    double x = startX + i * 5;
    double y = startY + amplitude * Math.Sin(i * 2 * Math.PI / wavelength);
    FreeNode point = new FreeNode(document, x, y);
    sourceSpline.Points.Add(point);
}

sourceSpline.Color = 255; // Красный цвет

// Создание симметрий с различными осями
int splineSymmetryCount = 4;
SymmetryConstruction[] splineSymmetries = new SymmetryConstruction[splineSymmetryCount];

for (int i = 0; i < splineSymmetryCount; i++)
{
    splineSymmetries[i] = new SymmetryConstruction(document);
    splineSymmetries[i].Source = sourceSpline;
    
    // Создание оси симметрии
    LineConstruction axis;
    switch (i)
    {
        case 0: // Вертикальная ось
            {
                FreeNode axisStart = new FreeNode(document, startX + (splinePoints * 5) / 2, startY - 20);
                FreeNode axisEnd = new FreeNode(document, startX + (splinePoints * 5) / 2, startY + 20);
                axis = new LineConstruction(document);
                axis.SetTwoNodes(axisStart, axisEnd);
                break;
            }
        case 1: // Горизонтальная ось
            {
                FreeNode axisStart = new FreeNode(document, startX - 10, startY);
                FreeNode axisEnd = new FreeNode(document, startX + splinePoints * 5 + 10, startY);
                axis = new LineConstruction(document);
                axis.SetTwoNodes(axisStart, axisEnd);
                break;
            }
        case 2: // Диагональная ось (45 градусов)
            {
                double centerX = startX + (splinePoints * 5) / 2;
                double centerY = startY;
                FreeNode axisStart = new FreeNode(document, centerX - 30, centerY - 30);
                FreeNode axisEnd = new FreeNode(document, centerX + 30, centerY + 30);
                axis = new LineConstruction(document);
                axis.SetTwoNodes(axisStart, axisEnd);
                break;
            }
        case 3: // Диагональная ось (-45 градусов)
            {
                double centerX = startX + (splinePoints * 5) / 2;
                double centerY = startY;
                FreeNode axisStart = new FreeNode(document, centerX - 30, centerY + 30);
                FreeNode axisEnd = new FreeNode(document, centerX + 30, centerY - 30);
                axis = new LineConstruction(document);
                axis.SetTwoNodes(axisStart, axisEnd);
                break;
            }
        default:
            axis = null;
            break;
    }
    
    if (axis != null)
    {
        axis.Color = 12632256; // Серый цвет
        axis.Style = LineStyle.Dash; // Пунктирная линия
        splineSymmetries[i].Axis = axis;
        splineSymmetries[i].Color = 65280; // Зеленый цвет
    }
}

// Создание симметрий с использованием точек
int pointSymmetryCount = 3;
SymmetryConstruction[] pointSymmetries = new SymmetryConstruction[pointSymmetryCount];
FreeNode[] symmetryPoints = new FreeNode[pointSymmetryCount];

for (int i = 0; i < pointSymmetryCount; i++)
{
    pointSymmetries[i] = new SymmetryConstruction(document);
    pointSymmetries[i].Source = sourceSpline;
    
    // Создание точек для определения осей симметрии
    double pointX = startX + 20 + i * 40;
    double pointY = startY - 30 + i * 30;
    symmetryPoints[i] = new FreeNode(document, pointX, pointY);
    
    // Создание оси симметрии через точку перпендикулярно к касательной
    // Для упрощения создаем ось через точку под определенным углом
    double angle = Math.PI * i / pointSymmetryCount;
    FreeNode axisStart = new FreeNode(document, pointX - 20 * Math.Cos(angle), pointY - 20 * Math.Sin(angle));
    FreeNode axisEnd = new FreeNode(document, pointX + 20 * Math.Cos(angle), pointY + 20 * Math.Sin(angle));
    LineConstruction axis = new LineConstruction(document);
    axis.SetTwoNodes(axisStart, axisEnd);
    axis.Color = 12632256; // Серый цвет
    axis.Style = LineStyle.DashDot; // Штрих-пунктирная линия
    
    pointSymmetries[i].Axis = axis;
    pointSymmetries[i].Color = 16711680; // Синий цвет
    
    // Создание визуальных маркеров точек
    CircleConstruction pointMarker = new CircleConstruction(document);
    pointMarker.SetCenterAndRadius(symmetryPoints[i], 2);
    pointMarker.Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание симметрий с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы симметрий");

// Создание исходных объектов (окружностей)
int circleCount = 4;
CircleConstruction[] sourceCircles = new CircleConstruction[circleCount];
FreeNode[] circleCenters = new FreeNode[circleCount];
double[] circleRadii = { 8, 12, 10, 15 };

for (int i = 0; i < circleCount; i++)
{
    double centerX = 40 + i * 30;
    double centerY = 50;
    circleCenters[i] = new FreeNode(document, centerX, centerY);
    sourceCircles[i] = new CircleConstruction(document);
    sourceCircles[i].SetCenterAndRadius(circleCenters[i], circleRadii[i]);
    sourceCircles[i].Color = 255; // Красный цвет
}

// Создание параметризованной системы симметрий
int paramSymmetryCount = 3;
SymmetryConstruction[,] circleSymmetries = new SymmetryConstruction[circleCount, paramSymmetryCount];
LineConstruction[,] symmetryAxes = new LineConstruction[circleCount, paramSymmetryCount];

for (int i = 0; i < circleCount; i++)
{
    for (int j = 0; j < paramSymmetryCount; j++)
    {
        circleSymmetries[i, j] = new SymmetryConstruction(document);
        circleSymmetries[i, j].Source = sourceCircles[i];
        
        // Создание оси симметрии под разными углами
        double angle = Math.PI * j / paramSymmetryCount;
        double axisLength = circleRadii[i] * 2;
        FreeNode axisStart = new FreeNode(document, 
            circleCenters[i].X.Value - axisLength * Math.Cos(angle), 
            circleCenters[i].Y.Value - axisLength * Math.Sin(angle));
        FreeNode axisEnd = new FreeNode(document, 
            circleCenters[i].X.Value + axisLength * Math.Cos(angle), 
            circleCenters[i].Y.Value + axisLength * Math.Sin(angle));
        
        symmetryAxes[i, j] = new LineConstruction(document);
        symmetryAxes[i, j].SetTwoNodes(axisStart, axisEnd);
        symmetryAxes[i, j].Color = 12632256; // Серый цвет
        symmetryAxes[i, j].Style = LineStyle.Dash; // Пунктирная линия
        
        circleSymmetries[i, j].Axis = symmetryAxes[i, j];
        
        // Установка цвета с градиентом
        int red = (int)(255 * (double)i / (circleCount - 1));
        int green = (int)(255 * (double)j / (paramSymmetryCount - 1));
        int blue = 255 - (red + green) / 2;
        circleSymmetries[i, j].Color = (red << 16) | (green << 8) | blue;
    }
}

// Создание симметрий для сложного контура
PathConstruction complexPath = new PathConstruction(document);

// Создание контура в форме неправильного многоугольника
FreeNode[] complexNodes = new FreeNode[6];
complexNodes[0] = new FreeNode(document, 30, 100);
complexNodes[1] = new FreeNode(document, 60, 95);
complexNodes[2] = new FreeNode(document, 70, 120);
complexNodes[3] = new FreeNode(document, 55, 140);
complexNodes[4] = new FreeNode(document, 35, 135);
complexNodes[5] = new FreeNode(document, 25, 120);

for (int i = 0; i < 6; i++)
{
    complexPath.AddSegment(complexNodes[i], complexNodes[(i + 1) % 6]);
}

complexPath.Color = 16711680; // Синий цвет

// Создание множественных симметрий для сложного контура
int complexSymmetryCount = 6;
SymmetryConstruction[] complexSymmetries = new SymmetryConstruction[complexSymmetryCount];
LineConstruction[] complexAxes = new LineConstruction[complexSymmetryCount];

// Вычисление центра контура
double centerX = 0, centerY = 0;
for (int i = 0; i < 6; i++)
{
    centerX += complexNodes[i].X.Value;
    centerY += complexNodes[i].Y.Value;
}
centerX /= 6;
centerY /= 6;

for (int i = 0; i < complexSymmetryCount; i++)
{
    complexSymmetries[i] = new SymmetryConstruction(document);
    complexSymmetries[i].Source = complexPath;
    
    // Создание осей симметрии через центр контура
    double angle = 2 * Math.PI * i / complexSymmetryCount;
    double axisLength = 40;
    FreeNode axisStart = new FreeNode(document, 
        centerX - axisLength * Math.Cos(angle), 
        centerY - axisLength * Math.Sin(angle));
    FreeNode axisEnd = new FreeNode(document, 
        centerX + axisLength * Math.Cos(angle), 
        centerY + axisLength * Math.Sin(angle));
    
    complexAxes[i] = new LineConstruction(document);
    complexAxes[i].SetTwoNodes(axisStart, axisEnd);
    complexAxes[i].Color = 12632256; // Серый цвет
    complexAxes[i].Style = LineStyle.DashDot; // Штрих-пунктирная линия
    
    complexSymmetries[i].Axis = complexAxes[i];
    complexSymmetries[i].Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция симметрий с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция симметрий с другими объектами");

// Создание исходного объекта (эллипса)
EllipseConstruction sourceEllipse = new EllipseConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
FreeNode majorNode = new FreeNode(document, 70, 50);
FreeNode minorNode = new FreeNode(document, 50, 65);
sourceEllipse.SetCenterAndTwoNodes(center, majorNode, minorNode);
sourceEllipse.Color = 255; // Красный цвет

// Создание симметрий, интегрированных с линиями
int integratedSymmetryCount = 4;
SymmetryConstruction[] integratedSymmetries = new SymmetryConstruction[integratedSymmetryCount];
LineConstruction[] symmetryAxes = new LineConstruction[integratedSymmetryCount];
LineConstruction[] connectionLines = new LineConstruction[integratedSymmetryCount];

for (int i = 0; i < integratedSymmetryCount; i++)
{
    integratedSymmetries[i] = new SymmetryConstruction(document);
    integratedSymmetries[i].Source = sourceEllipse;
    
    // Создание осей симметрии под разными углами
    double angle = Math.PI * i / integratedSymmetryCount;
    double axisLength = 40;
    FreeNode axisStart = new FreeNode(document, 
        center.X.Value - axisLength * Math.Cos(angle), 
        center.Y.Value - axisLength * Math.Sin(angle));
    FreeNode axisEnd = new FreeNode(document, 
        center.X.Value + axisLength * Math.Cos(angle), 
        center.Y.Value + axisLength * Math.Sin(angle));
    
    symmetryAxes[i] = new LineConstruction(document);
    symmetryAxes[i].SetTwoNodes(axisStart, axisEnd);
    symmetryAxes[i].Color = 12632256; // Серый цвет
    symmetryAxes[i].Style = LineStyle.Dash; // Пунктирная линия
    
    integratedSymmetries[i].Axis = symmetryAxes[i];
    integratedSymmetries[i].Color = 65280; // Зеленый цвет
    
    // Создание соединительных линий от центра к концам осей
    connectionLines[i * 2] = new LineConstruction(document);
    connectionLines[i * 2].SetTwoNodes(center, axisStart);
    connectionLines[i * 2].Color = 16711680; // Синий цвет
    connectionLines[i * 2].Style = LineStyle.Dot; // Точечная линия
    
    connectionLines[i * 2 + 1] = new LineConstruction(document);
    connectionLines[i * 2 + 1].SetTwoNodes(center, axisEnd);
    connectionLines[i * 2 + 1].Color = 16711680; // Синий цвет
    connectionLines[i * 2 + 1].Style = LineStyle.Dot; // Точечная линия
}

// Создание симметрий, интегрированных с контурами
PathConstruction referencePath = new PathConstruction(document);

// Создание контура в форме прямоугольника
FreeNode[] rectangleNodes = new FreeNode[4];
rectangleNodes[0] = new FreeNode(document, 120, 30);
rectangleNodes[1] = new FreeNode(document, 170, 30);
rectangleNodes[2] = new FreeNode(document, 170, 80);
rectangleNodes[3] = new FreeNode(document, 120, 80);

for (int i = 0; i < 4; i++)
{
    referencePath.AddSegment(rectangleNodes[i], rectangleNodes[(i + 1) % 4]);
}

referencePath.Color = 16711680; // Синий цвет

// Создание симметрий для контура
int pathSymmetryCount = 2;
SymmetryConstruction[] pathSymmetries = new SymmetryConstruction[pathSymmetryCount];
LineConstruction[] pathAxes = new LineConstruction[pathSymmetryCount];

for (int i = 0; i < pathSymmetryCount; i++)
{
    pathSymmetries[i] = new SymmetryConstruction(document);
    pathSymmetries[i].Source = referencePath;
    
    // Создание осей симметрии (вертикальная и горизонтальная)
    FreeNode axisStart, axisEnd;
    if (i == 0)
    {
        // Вертикальная ось
        axisStart = new FreeNode(document, 145, 20);
        axisEnd = new FreeNode(document, 145, 90);
    }
    else
    {
        // Горизонтальная ось
        axisStart = new FreeNode(document, 110, 55);
        axisEnd = new FreeNode(document, 180, 55);
    }
    
    pathAxes[i] = new LineConstruction(document);
    pathAxes[i].SetTwoNodes(axisStart, axisEnd);
    pathAxes[i].Color = 12632256; // Серый цвет
    pathAxes[i].Style = LineStyle.DashDot; // Штрих-пунктирная линия
    
    pathSymmetries[i].Axis = pathAxes[i];
    pathSymmetries[i].Color = 16776960; // Желтый цвет
}

// Создание симметрий, интегрированных с другими симметриями
SymmetryConstruction[] secondarySymmetries = new SymmetryConstruction[2];

for (int i = 0; i < 2; i++)
{
    secondarySymmetries[i] = new SymmetryConstruction(document);
    secondarySymmetries[i].Source = integratedSymmetries[i]; // Используем существующие симметрии
    
    // Создание перпендикулярных осей
    double angle = Math.PI * i / 2 + Math.PI / 2;
    double axisLength = 30;
    FreeNode axisStart = new FreeNode(document, 
        center.X.Value - axisLength * Math.Cos(angle), 
        center.Y.Value - axisLength * Math.Sin(angle));
    FreeNode axisEnd = new FreeNode(document, 
        center.X.Value + axisLength * Math.Cos(angle), 
        center.Y.Value + axisLength * Math.Sin(angle));
    
    LineConstruction axis = new LineConstruction(document);
    axis.SetTwoNodes(axisStart, axisEnd);
    axis.Color = 12632256; // Серый цвет
    axis.Style = LineStyle.Dash; // Пунктирная линия
    
    secondarySymmetries[i].Axis = axis;
    secondarySymmetries[i].Color = 16711935; // Пурпурный цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством симметрий

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества симметрий с минимальными вызовами API
int symmetryCount = 100;
SymmetryConstruction[] symmetries = new SymmetryConstruction[symmetryCount];

// Создание исходных объектов (простых линий)
LineConstruction[] sourceLines = new LineConstruction[20];
FreeNode[,] lineNodes = new FreeNode[20, 2];

Random random = new Random();
for (int i = 0; i < 20; i++)
{
    sourceLines[i] = new LineConstruction(document);
    lineNodes[i, 0] = new FreeNode(document, 
        20 + random.NextDouble() * 160, 
        20 + random.NextDouble() * 110);
    lineNodes[i, 1] = new FreeNode(document, 
        lineNodes[i, 0].X.Value + 10 + random.NextDouble() * 20, 
        lineNodes[i, 0].Y.Value + 10 + random.NextDouble() * 20);
    sourceLines[i].SetTwoNodes(lineNodes[i, 0], lineNodes[i, 1]);
    sourceLines[i].Color = 255; // Красный цвет
}

// Предварительное создание осей симметрии
LineConstruction[] symmetryAxes = new LineConstruction[symmetryCount];
FreeNode[,] axisNodes = new FreeNode[symmetryCount, 2];

for (int i = 0; i < symmetryCount; i++)
{
    axisNodes[i, 0] = new FreeNode(document, 
        10 + random.NextDouble() * 180, 
        10 + random.NextDouble() * 130);
    axisNodes[i, 1] = new FreeNode(document, 
        axisNodes[i, 0].X.Value + 20 + random.NextDouble() * 40, 
        axisNodes[i, 0].Y.Value + 20 + random.NextDouble() * 40);
    
    symmetryAxes[i] = new LineConstruction(document);
    symmetryAxes[i].SetTwoNodes(axisNodes[i, 0], axisNodes[i, 1]);
    symmetryAxes[i].Color = 12632256; // Серый цвет
    symmetryAxes[i].Style = LineStyle.Dash; // Пунктирная линия
}

// Создание симметрий
for (int i = 0; i < symmetryCount; i++)
{
    symmetries[i] = new SymmetryConstruction(document);
    symmetries[i].Source = sourceLines[i % 20];
    symmetries[i].Axis = symmetryAxes[i];
    
    // Установка цвета
    int red = (int)(255 * random.NextDouble());
    int green = (int)(255 * random.NextDouble());
    int blue = (int)(255 * random.NextDouble());
    symmetries[i].Color = (red << 16) | (green << 8) | blue;
    
    // Установка толщины линии
    symmetries[i].LineWidth = 1 + (int)(random.NextDouble() * 2);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими симметриями и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические симметрии");

// Создание исходного объекта с возможностью динамического обновления
CircleConstruction dynamicSource = new CircleConstruction(document);
FreeNode dynamicCenter = new FreeNode(document, 50, 50);
dynamicSource.SetCenterAndRadius(dynamicCenter, 12);
dynamicSource.Color = 255; // Красный цвет

// Создание симметрий с возможностью динамического обновления
int dynamicSymmetryCount = 4;
SymmetryConstruction[] dynamicSymmetries = new SymmetryConstruction[dynamicSymmetryCount];
LineConstruction[] dynamicAxes = new LineConstruction[dynamicSymmetryCount];
FreeNode[,] axisEndpoints = new FreeNode[dynamicSymmetryCount, 2];

for (int i = 0; i < dynamicSymmetryCount; i++)
{
    dynamicSymmetries[i] = new SymmetryConstruction(document);
    dynamicSymmetries[i].Source = dynamicSource;
    
    // Создание осей симметрии с возможностью обновления
    axisEndpoints[i, 0] = new FreeNode(document, 
        50 - 30 * Math.Cos(Math.PI * i / dynamicSymmetryCount), 
        50 - 30 * Math.Sin(Math.PI * i / dynamicSymmetryCount));
    axisEndpoints[i, 1] = new FreeNode(document, 
        50 + 30 * Math.Cos(Math.PI * i / dynamicSymmetryCount), 
        50 + 30 * Math.Sin(Math.PI * i / dynamicSymmetryCount));
    
    dynamicAxes[i] = new LineConstruction(document);
    dynamicAxes[i].SetTwoNodes(axisEndpoints[i, 0], axisEndpoints[i, 1]);
    dynamicAxes[i].Color = 12632256; // Серый цвет
    dynamicAxes[i].Style = LineStyle.Dash; // Пунктирная линия
    
    dynamicSymmetries[i].Axis = dynamicAxes[i];
    dynamicSymmetries[i].Color = 65280; // Зеленый цвет
}

// Создание симметрий, которые будут менять свои параметры
SymmetryConstruction[] morphingSymmetries = new SymmetryConstruction[3];
LineConstruction[] morphingAxes = new LineConstruction[3];
EllipseConstruction[] morphingSources = new EllipseConstruction[3];

for (int i = 0; i < 3; i++)
{
    morphingSymmetries[i] = new SymmetryConstruction(document);
    
    // Создание отдельных эллипсов для каждой симметрии
    double centerX = 120 + i * 40;
    double centerY = 50;
    FreeNode center = new FreeNode(document, centerX, centerY);
    FreeNode majorNode = new FreeNode(document, centerX + 15, centerY);
    FreeNode minorNode = new FreeNode(document, centerX, centerY + 10);
    morphingSources[i] = new EllipseConstruction(document);
    morphingSources[i].SetCenterAndTwoNodes(center, majorNode, minorNode);
    morphingSymmetries[i].Source = morphingSources[i];
    
    // Создание осей симметрии
    FreeNode axisStart = new FreeNode(document, centerX - 25, centerY);
    FreeNode axisEnd = new FreeNode(document, centerX + 25, centerY);
    morphingAxes[i] = new LineConstruction(document);
    morphingAxes[i].SetTwoNodes(axisStart, axisEnd);
    morphingAxes[i].Color = 12632256; // Серый цвет
    morphingAxes[i].Style = LineStyle.DashDot; // Штрих-пунктирная линия
    
    morphingSymmetries[i].Axis = morphingAxes[i];
    morphingSymmetries[i].Color = 16711680; // Синий цвет
}

// Создание системы симметрий с анимацией
int animatedSymmetryCount = 6;
SymmetryConstruction[] animatedSymmetries = new SymmetryConstruction[animatedSymmetryCount];
LineConstruction[] animatedAxes = new LineConstruction[animatedSymmetryCount];
PathConstruction[] animatedSources = new PathConstruction[animatedSymmetryCount];

for (int i = 0; i < animatedSymmetryCount; i++)
{
    animatedSymmetries[i] = new SymmetryConstruction(document);
    
    // Создание отдельных контуров для анимированных симметрий
    animatedSources[i] = new PathConstruction(document);
    
    // Создание ромбовидных контуров
    double centerX = 50 + 80 * Math.Cos(2 * Math.PI * i / animatedSymmetryCount);
    double centerY = 50 + 80 * Math.Sin(2 * Math.PI * i / animatedSymmetryCount);
    FreeNode[] nodes = new FreeNode[4];
    nodes[0] = new FreeNode(document, centerX, centerY - 10);
    nodes[1] = new FreeNode(document, centerX + 10, centerY);
    nodes[2] = new FreeNode(document, centerX, centerY + 10);
    nodes[3] = new FreeNode(document, centerX - 10, centerY);
    
    for (int j = 0; j < 4; j++)
    {
        animatedSources[i].AddSegment(nodes[j], nodes[(j + 1) % 4]);
    }
    
    animatedSymmetries[i].Source = animatedSources[i];
    
    // Создание осей симметрии
    FreeNode axisStart = new FreeNode(document, centerX - 20, centerY);
    FreeNode axisEnd = new FreeNode(document, centerX + 20, centerY);
    animatedAxes[i] = new LineConstruction(document);
    animatedAxes[i].SetTwoNodes(axisStart, axisEnd);
    animatedAxes[i].Color = 12632256; // Серый цвет
    animatedAxes[i].Style = LineStyle.Dash; // Пунктирная линия
    
    animatedSymmetries[i].Axis = animatedAxes[i];
    animatedSymmetries[i].Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств симметрий
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicSymmetries(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических симметрий");
    
    // Обновление центра исходного объекта
    double newX = 50 + 10 * Math.Sin(time * 0.3);
    double newY = 50 + 10 * Math.Cos(time * 0.3);
    dynamicCenter.X.Value = newX;
    dynamicCenter.Y.Value = newY;
    
    // Обновление осей динамических симметрий
    for (int i = 0; i < dynamicSymmetryCount; i++)
    {
        double angle = Math.PI * i / dynamicSymmetryCount + time * 0.2;
        axisEndpoints[i, 0].X.Value = 50 - 30 * Math.Cos(angle);
        axisEndpoints[i, 0].Y.Value = 50 - 30 * Math.Sin(angle);
        axisEndpoints[i, 1].X.Value = 50 + 30 * Math.Cos(angle);
        axisEndpoints[i, 1].Y.Value = 50 + 30 * Math.Sin(angle);
    }
    
    // Обновление параметров морфирующих симметрий
    for (int i = 0; i < 3; i++)
    {
        double newMajor = 15 + 5 * Math.Sin(time * 0.5 + i);
        double newMinor = 10 + 5 * Math.Cos(time * 0.5 + i);
        // В реальной реализации потребуется способ обновления параметров исходных эллипсов
        // morphingSources[i].SetCenterAndTwoNodes(...);
        
        // Изменение цвета
        int red = (int)(255 * (1 + Math.Sin(time * 0.5 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.5 + i + Math.PI / 3)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.5 + i + 2 * Math.PI / 3)) / 2);
        morphingSymmetries[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Обновление анимированных симметрий
    for (int i = 0; i < animatedSymmetryCount; i++)
    {
        double centerX = 50 + 80 * Math.Cos(2 * Math.PI * i / animatedSymmetryCount + time * 0.1);
        double centerY = 50 + 80 * Math.Sin(2 * Math.PI * i / animatedSymmetryCount + time * 0.1);
        
        // Обновление узлов контура
        animatedSources[i].Segments.Clear();
        FreeNode[] nodes = new FreeNode[4];
        nodes[0] = new FreeNode(document, centerX, centerY - 10);
        nodes[1] = new FreeNode(document, centerX + 10, centerY);
        nodes[2] = new FreeNode(document, centerX, centerY + 10);
        nodes[3] = new FreeNode(document, centerX - 10, centerY);
        
        for (int j = 0; j < 4; j++)
        {
            animatedSources[i].AddSegment(nodes[j], nodes[(j + 1) % 4]);
        }
        
        // Обновление осей симметрии
        animatedAxes[i].SetTwoNodes(
            new FreeNode(document, centerX - 20, centerY),
            new FreeNode(document, centerX + 20, centerY));
        
        // Изменение цвета в зависимости от времени
        int red = (int)(255 * (1 + Math.Sin(time * 0.2 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.2 + i + 1)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.2 + i + 2)) / 2);
        animatedSymmetries[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
```

## Свойства и методы

### Основные свойства:

- `Source` - Исходная линия построения
- `Axis` - Ось симметрии
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

### Основные методы:

- `SetSource` - Установка исходного объекта
- `SetAxis` - Установка оси симметрии
- `GetSymmetricGeometry` - Получение геометрии симметричного объекта

## Заключение

Продвинутое использование класса `SymmetryConstruction` включает в себя создание сложных симметричных конструкций, применение геометрических расчетов, параметризованные конструкции, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами симметрий важно учитывать производительность и использовать эффективные алгоритмы для вычисления симметричных копий и установления связей между объектами.
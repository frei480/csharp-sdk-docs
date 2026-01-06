# OffsetConstruction - продвинутые примеры использования

Класс `OffsetConstruction` представляет линию построения-эквидистанту в T-Flex CAD API. Этот класс предоставляет возможности для создания параллельных копий объектов на заданном расстоянии.

## Продвинутые примеры использования

### 1. Создание сложных систем эквидистант

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сложных систем эквидистант");

// Создание исходного контура (звезды)
PathConstruction sourceStar = new PathConstruction(document);

int starPoints = 6;
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

// Создание множественных эквидистант
int offsetCount = 5;
double[] offsets = { 5, 10, 15, 20, 25 };
int[] colors = { 65280, 16711680, 16776960, 65535, 16711935 };

OffsetConstruction[] starOffsets = new OffsetConstruction[offsetCount];

for (int i = 0; i < offsetCount; i++)
{
    starOffsets[i] = new OffsetConstruction(document);
    starOffsets[i].Source = sourceStar;
    starOffsets[i].Offset = offsets[i];
    starOffsets[i].Color = colors[i];
    starOffsets[i].LineWidth = 2;
}

// Создание эквидистант с переменным смещением
int variableOffsetCount = 8;
OffsetConstruction[] variableOffsets = new OffsetConstruction[variableOffsetCount];

for (int i = 0; i < variableOffsetCount; i++)
{
    variableOffsets[i] = new OffsetConstruction(document);
    variableOffsets[i].Source = sourceStar;
    
    // Переменное смещение
    double variableOffset = 5 + 20 * Math.Sin(2 * Math.PI * i / variableOffsetCount);
    variableOffsets[i].Offset = variableOffset;
    
    // Установка цвета в зависимости от смещения
    int intensity = (int)(255 * (variableOffset - 5) / 20);
    variableOffsets[i].Color = (intensity << 16) | ((255 - intensity) << 8) | 128;
    variableOffsets[i].LineWidth = 1 + i / 3;
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание эквидистант с геометрическими расчетами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание эквидистант с геометрическими расчетами");

// Создание исходного сложного сплайна
SplineConstruction sourceSpline = new SplineConstruction(document);

// Создание точек сплайна в форме S-кривой
double startX = 30;
double startY = 30;
int splinePoints = 15;

for (int i = 0; i <= splinePoints; i++)
{
    double t = (double)i / splinePoints;
    double x = startX + t * 100;
    double y = startY + 30 * Math.Sin(Math.PI * t);
    FreeNode point = new FreeNode(document, x, y);
    sourceSpline.Points.Add(point);
}

sourceSpline.Color = 255; // Красный цвет

// Создание эквидистант с различными смещениями
int splineOffsetCount = 6;
double[] splineOffsets = { -10, -5, 5, 10, 15, 20 };
int[] splineColors = { 65280, 65535, 16776960, 16711680, 16711935, 255 };

OffsetConstruction[] splineOffsetsArray = new OffsetConstruction[splineOffsetCount];

for (int i = 0; i < splineOffsetCount; i++)
{
    splineOffsetsArray[i] = new OffsetConstruction(document);
    splineOffsetsArray[i].Source = sourceSpline;
    splineOffsetsArray[i].Offset = splineOffsets[i];
    splineOffsetsArray[i].Color = splineColors[i];
    
    // Установка толщины линии в зависимости от смещения
    splineOffsetsArray[i].LineWidth = 1 + Math.Abs(splineOffsets[i]) / 10;
}

// Создание эквидистант с использованием узлов смещения
int nodeOffsetCount = 4;
OffsetConstruction[] nodeOffsets = new OffsetConstruction[nodeOffsetCount];
FreeNode[] offsetNodes = new FreeNode[nodeOffsetCount];

for (int i = 0; i < nodeOffsetCount; i++)
{
    nodeOffsets[i] = new OffsetConstruction(document);
    nodeOffsets[i].Source = sourceSpline;
    
    // Создание узла для определения смещения
    double nodeX = 50 + i * 20;
    double nodeY = 80 + i * 10;
    offsetNodes[i] = new FreeNode(document, nodeX, nodeY);
    nodeOffsets[i].OffsetNode = offsetNodes[i];
    nodeOffsets[i].Color = 16711680; // Синий цвет
    
    // Создание визуальных маркеров узлов смещения
    CircleConstruction nodeMarker = new CircleConstruction(document);
    nodeMarker.SetCenterAndRadius(offsetNodes[i], 2);
    nodeMarker.Color = 16776960; // Желтый цвет
}

// Создание эквидистант с переменной толщиной
OffsetConstruction variableWidthOffset = new OffsetConstruction(document);
variableWidthOffset.Source = sourceSpline;
variableWidthOffset.Offset = 12;

// В реальной реализации переменная толщина может быть установлена через дополнительные параметры
// Здесь устанавливаем фиксированную толщину для демонстрации
variableWidthOffset.LineWidth = 3;
variableWidthOffset.Color = 65280; // Зеленый цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание эквидистант с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы эквидистант");

// Создание исходных объектов (окружностей)
int circleCount = 5;
CircleConstruction[] sourceCircles = new CircleConstruction[circleCount];
FreeNode[] circleCenters = new FreeNode[circleCount];
double[] circleRadii = { 10, 15, 12, 18, 14 };

for (int i = 0; i < circleCount; i++)
{
    double centerX = 40 + i * 25;
    double centerY = 50;
    circleCenters[i] = new FreeNode(document, centerX, centerY);
    sourceCircles[i] = new CircleConstruction(document);
    sourceCircles[i].SetCenterAndRadius(circleCenters[i], circleRadii[i]);
    sourceCircles[i].Color = 255; // Красный цвет
}

// Создание параметризованной системы эквидистант
int paramOffsetCount = 4;
OffsetConstruction[,] circleOffsets = new OffsetConstruction[circleCount, paramOffsetCount];

for (int i = 0; i < circleCount; i++)
{
    for (int j = 0; j < paramOffsetCount; j++)
    {
        circleOffsets[i, j] = new OffsetConstruction(document);
        circleOffsets[i, j].Source = sourceCircles[i];
        
        // Параметрическое смещение
        double offset = 5 + j * 8;
        circleOffsets[i, j].Offset = offset;
        
        // Установка цвета с градиентом
        int red = (int)(255 * (double)i / (circleCount - 1));
        int green = (int)(255 * (double)j / (paramOffsetCount - 1));
        int blue = 255 - (red + green) / 2;
        circleOffsets[i, j].Color = (red << 16) | (green << 8) | blue;
        
        // Установка толщины линии
        circleOffsets[i, j].LineWidth = 1 + j;
    }
}

// Создание эквидистант для сложного контура
PathConstruction complexPath = new PathConstruction(document);

// Создание контура в форме неправильного многоугольника
FreeNode[] complexNodes = new FreeNode[7];
complexNodes[0] = new FreeNode(document, 30, 100);
complexNodes[1] = new FreeNode(document, 60, 95);
complexNodes[2] = new FreeNode(document, 70, 120);
complexNodes[3] = new FreeNode(document, 55, 140);
complexNodes[4] = new FreeNode(document, 35, 135);
complexNodes[5] = new FreeNode(document, 25, 120);
complexNodes[6] = new FreeNode(document, 20, 110);

for (int i = 0; i < 7; i++)
{
    complexPath.AddSegment(complexNodes[i], complexNodes[(i + 1) % 7]);
}

complexPath.Color = 16711680; // Синий цвет

// Создание множественных эквидистант для сложного контура
int complexOffsetCount = 5;
double[] complexOffsets = { -8, -4, 4, 8, 12 };
int[] complexColors = { 65280, 65535, 16776960, 16711935, 255 };

OffsetConstruction[] complexOffsetsArray = new OffsetConstruction[complexOffsetCount];

for (int i = 0; i < complexOffsetCount; i++)
{
    complexOffsetsArray[i] = new OffsetConstruction(document);
    complexOffsetsArray[i].Source = complexPath;
    complexOffsetsArray[i].Offset = complexOffsets[i];
    complexOffsetsArray[i].Color = complexColors[i];
    complexOffsetsArray[i].LineWidth = 2;
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция эквидистант с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция эквидистант с другими объектами");

// Создание исходного объекта (эллипса)
EllipseConstruction sourceEllipse = new EllipseConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
FreeNode majorNode = new FreeNode(document, 70, 50);
FreeNode minorNode = new FreeNode(document, 50, 65);
sourceEllipse.SetCenterAndTwoNodes(center, majorNode, minorNode);
sourceEllipse.Color = 255; // Красный цвет

// Создание эквидистант, интегрированных с линиями
int integratedOffsetCount = 8;
OffsetConstruction[] integratedOffsets = new OffsetConstruction[integratedOffsetCount];
LineConstruction[] connectionLines = new LineConstruction[integratedOffsetCount];

for (int i = 0; i < integratedOffsetCount; i++)
{
    integratedOffsets[i] = new OffsetConstruction(document);
    integratedOffsets[i].Source = sourceEllipse;
    
    // Переменное смещение
    double offset = 10 + 15 * Math.Sin(2 * Math.PI * i / integratedOffsetCount);
    integratedOffsets[i].Offset = offset;
    integratedOffsets[i].Color = 65280; // Зеленый цвет
    
    // Создание соединительных линий от центра к точкам эквидистант
    double angle = 2 * Math.PI * i / integratedOffsetCount;
    double connectionX = center.X.Value + (20 + offset) * Math.Cos(angle);
    double connectionY = center.Y.Value + (15 + offset) * Math.Sin(angle);
    FreeNode connectionPoint = new FreeNode(document, connectionX, connectionY);
    connectionLines[i] = new LineConstruction(document);
    connectionLines[i].SetTwoNodes(center, connectionPoint);
    connectionLines[i].Color = 12632256; // Серый цвет
    connectionLines[i].Style = LineStyle.Dash; // Пунктирная линия
}

// Создание эквидистант, интегрированных с контурами
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

// Создание эквидистант для контура
OffsetConstruction pathOffset = new OffsetConstruction(document);
pathOffset.Source = referencePath;
pathOffset.Offset = 10;
pathOffset.Color = 16776960; // Желтый цвет

// Создание точек на эквидистанте
int pointsOnOffset = 12;
FreeNode[] offsetPoints = new FreeNode[pointsOnOffset];

for (int i = 0; i < pointsOnOffset; i++)
{
    // В реальной реализации здесь потребуется вычисление точек на эквидистанте
    // Для упрощения примера создаем точки вручную
    double t = (double)i / (pointsOnOffset - 1);
    double x = 120 + t * 50 + 10 * Math.Cos(2 * Math.PI * t);
    double y = 30 + t * 50 + 10 * Math.Sin(2 * Math.PI * t);
    offsetPoints[i] = new FreeNode(document, x, y);
    
    // Создание визуальных маркеров точек
    CircleConstruction pointMarker = new CircleConstruction(document);
    pointMarker.SetCenterAndRadius(offsetPoints[i], 1.5);
    pointMarker.Color = 16711935; // Пурпурный цвет
}

// Создание эквидистант, интегрированных с другими эквидистантами
OffsetConstruction[] secondaryOffsets = new OffsetConstruction[4];

for (int i = 0; i < 4; i++)
{
    secondaryOffsets[i] = new OffsetConstruction(document);
    secondaryOffsets[i].Source = integratedOffsets[i * 2]; // Используем каждую вторую эквидистанту
    
    // Смещение относительно исходной эквидистанты
    secondaryOffsets[i].Offset = 5;
    secondaryOffsets[i].Color = 255; // Красный цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством эквидистант

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества эквидистант с минимальными вызовами API
int offsetCount = 150;
OffsetConstruction[] offsets = new OffsetConstruction[offsetCount];

// Создание исходных объектов (простых линий)
LineConstruction[] sourceLines = new LineConstruction[50];
FreeNode[,] lineNodes = new FreeNode[50, 2];

Random random = new Random();
for (int i = 0; i < 50; i++)
{
    sourceLines[i] = new LineConstruction(document);
    lineNodes[i, 0] = new FreeNode(document, 
        20 + random.NextDouble() * 160, 
        20 + random.NextDouble() * 110);
    lineNodes[i, 1] = new FreeNode(document, 
        lineNodes[i, 0].X.Value + 10 + random.NextDouble() * 20, 
        lineNodes[i, 0].Y.Value + 10 + random.NextDouble() * 20);
    sourceLines[i].SetTwoNodes(lineNodes[i, 0], lineNodes[i, 1]);
}

// Создание эквидистант
for (int i = 0; i < offsetCount; i++)
{
    offsets[i] = new OffsetConstruction(document);
    offsets[i].Source = sourceLines[i % 50];
    
    // Случайное смещение
    double offset = 5 + random.NextDouble() * 20;
    offsets[i].Offset = offset;
    
    // Установка цвета
    int red = (int)(255 * random.NextDouble());
    int green = (int)(255 * random.NextDouble());
    int blue = (int)(255 * random.NextDouble());
    offsets[i].Color = (red << 16) | (green << 8) | blue;
    
    // Установка толщины линии
    offsets[i].LineWidth = 1 + (int)(random.NextDouble() * 3);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими эквидистантами и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические эквидистанты");

// Создание исходного объекта с возможностью динамического обновления
CircleConstruction dynamicSource = new CircleConstruction(document);
FreeNode dynamicCenter = new FreeNode(document, 50, 50);
dynamicSource.SetCenterAndRadius(dynamicCenter, 15);
dynamicSource.Color = 255; // Красный цвет

// Создание эквидистант с возможностью динамического обновления
int dynamicOffsetCount = 6;
OffsetConstruction[] dynamicOffsets = new OffsetConstruction[dynamicOffsetCount];
double[] baseOffsets = { 5, 10, 15, 20, 25, 30 };

for (int i = 0; i < dynamicOffsetCount; i++)
{
    dynamicOffsets[i] = new OffsetConstruction(document);
    dynamicOffsets[i].Source = dynamicSource;
    dynamicOffsets[i].Offset = baseOffsets[i];
    dynamicOffsets[i].Color = 65280; // Зеленый цвет
}

// Создание эквидистант, которые будут менять свои параметры
OffsetConstruction[] morphingOffsets = new OffsetConstruction[4];
FreeNode[] morphingCenters = new FreeNode[4];

for (int i = 0; i < 4; i++)
{
    morphingOffsets[i] = new OffsetConstruction(document);
    
    // Создание отдельных окружностей для каждой эквидистанты
    double centerX = 120 + i * 30;
    double centerY = 50;
    morphingCenters[i] = new FreeNode(document, centerX, centerY);
    CircleConstruction morphingSource = new CircleConstruction(document);
    morphingSource.SetCenterAndRadius(morphingCenters[i], 10);
    morphingOffsets[i].Source = morphingSource;
    
    morphingOffsets[i].Offset = 8;
    morphingOffsets[i].Color = 16711680; // Синий цвет
}

// Создание системы эквидистант с анимацией
int animatedOffsetCount = 8;
OffsetConstruction[] animatedOffsets = new OffsetConstruction[animatedOffsetCount];
double[] animatedBaseOffsets = new double[animatedOffsetCount];

for (int i = 0; i < animatedOffsetCount; i++)
{
    animatedOffsets[i] = new OffsetConstruction(document);
    
    // Создание отдельных эллипсов для анимированных эквидистант
    double centerX = 50 + 80 * Math.Cos(2 * Math.PI * i / animatedOffsetCount);
    double centerY = 50 + 80 * Math.Sin(2 * Math.PI * i / animatedOffsetCount);
    FreeNode animatedCenter = new FreeNode(document, centerX, centerY);
    EllipseConstruction animatedSource = new EllipseConstruction(document);
    FreeNode majorNode = new FreeNode(document, centerX + 12, centerY);
    FreeNode minorNode = new FreeNode(document, centerX, centerY + 8);
    animatedSource.SetCenterAndTwoNodes(animatedCenter, majorNode, minorNode);
    animatedOffsets[i].Source = animatedSource;
    
    animatedBaseOffsets[i] = 6;
    animatedOffsets[i].Offset = animatedBaseOffsets[i];
    animatedOffsets[i].Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств эквидистант
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicOffsets(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических эквидистант");
    
    // Обновление центра исходного объекта
    double newX = 50 + 15 * Math.Sin(time * 0.3);
    double newY = 50 + 15 * Math.Cos(time * 0.3);
    dynamicCenter.X.Value = newX;
    dynamicCenter.Y.Value = newY;
    
    // Обновление смещений динамических эквидистант
    for (int i = 0; i < dynamicOffsetCount; i++)
    {
        double animatedOffset = baseOffsets[i] + 5 * Math.Sin(time * 0.5 + i);
        dynamicOffsets[i].Offset = animatedOffset;
    }
    
    // Обновление параметров морфирующих эквидистант
    for (int i = 0; i < 4; i++)
    {
        double newRadius = 10 + 5 * Math.Sin(time * 0.7 + i);
        // В реальной реализации потребуется способ обновления радиуса исходной окружности
        // morphingSources[i].SetCenterAndRadius(morphingCenters[i], newRadius);
        
        // Изменение цвета
        int red = (int)(255 * (1 + Math.Sin(time * 0.7 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.7 + i + Math.PI / 3)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.7 + i + 2 * Math.PI / 3)) / 2);
        morphingOffsets[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Обновление анимированных эквидистант
    for (int i = 0; i < animatedOffsetCount; i++)
    {
        double newOffset = animatedBaseOffsets[i] + 3 * Math.Sin(time * 0.4 + i);
        animatedOffsets[i].Offset = newOffset;
        
        // Изменение цвета в зависимости от времени
        int red = (int)(255 * (1 + Math.Sin(time * 0.2 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.2 + i + 1)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.2 + i + 2)) / 2);
        animatedOffsets[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
```

## Свойства и методы

### Основные свойства:

- `Source` - Исходная линия построения
- `Offset` - Смещение эквидистанты
- `OffsetNode` - Узел, задающий смещение
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
- `SetOffset` - Установка смещения
- `SetOffsetNode` - Установка узла смещения
- `GetOffsetGeometry` - Получение геометрии эквидистанты

## Заключение

Продвинутое использование класса `OffsetConstruction` включает в себя создание сложных систем эквидистант, применение геометрических расчетов, параметризованные конструкции, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами эквидистант важно учитывать производительность и использовать эффективные алгоритмы для вычисления смещений и установления связей между объектами.
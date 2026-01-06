# SplineConstruction - продвинутые примеры использования

Класс `SplineConstruction` представляет сплайн построения в T-Flex CAD API. Этот класс предоставляет возможности для создания сложных кривых, проходящих через заданные точки.

## Продвинутые примеры использования

### 1. Создание сложных сплайнов с множеством точек

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сложных сплайнов");

// Создание сплайна в форме восьмерки
SplineConstruction figureEightSpline = new SplineConstruction(document);

// Определение точек для восьмерки
double centerX = 50;
double centerY = 50;
double radius = 20;

for (int i = 0; i <= 36; i++)
{
    double t = i * Math.PI / 18; // 36 точек на 2π
    double x = centerX + radius * Math.Sin(2 * t);
    double y = centerY + radius * Math.Sin(t);
    FreeNode point = new FreeNode(document, x, y);
    figureEightSpline.Points.Add(point);
}

figureEightSpline.IsClosed = true; // Замкнутый сплайн
figureEightSpline.Color = 255; // Красный цвет

// Создание сплайна в форме спирали
SplineConstruction spiralSpline = new SplineConstruction(document);

// Определение точек для спирали
int spiralPoints = 50;
double spiralRadius = 5;

for (int i = 0; i < spiralPoints; i++)
{
    double angle = i * 0.5;
    double radius = spiralRadius + i * 0.5;
    double x = centerX + 60 + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    FreeNode point = new FreeNode(document, x, y);
    spiralSpline.Points.Add(point);
}

spiralSpline.Color = 65280; // Зеленый цвет

// Создание сплайна в форме волны
SplineConstruction waveSpline = new SplineConstruction(document);

// Определение точек для волны
int wavePoints = 40;
double waveAmplitude = 10;
double waveLength = 5;

for (int i = 0; i <= wavePoints; i++)
{
    double x = 20 + i * 3;
    double y = centerY + 30 + waveAmplitude * Math.Sin(i * 2 * Math.PI / waveLength);
    FreeNode point = new FreeNode(document, x, y);
    waveSpline.Points.Add(point);
}

waveSpline.Color = 16711680; // Синий цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание сплайнов с геометрическими расчетами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сплайнов с геометрическими расчетами");

// Создание сплайна, огибающего набор точек (выпуклая оболочка)
SplineConstruction convexHullSpline = new SplineConstruction(document);

// Создание случайных точек
int pointCount = 20;
FreeNode[] points = new FreeNode[pointCount];
Random random = new Random();

for (int i = 0; i < pointCount; i++)
{
    double x = 30 + random.NextDouble() * 100;
    double y = 30 + random.NextDouble() * 80;
    points[i] = new FreeNode(document, x, y);
    
    // Создание визуальных маркеров точек
    CircleConstruction pointMarker = new CircleConstruction(document);
    pointMarker.SetCenterAndRadius(points[i], 1);
    pointMarker.Color = 12632256; // Серый цвет
}

// Для упрощения примера создаем сплайн, проходящий через все точки
// В реальной реализации здесь потребуется алгоритм построения выпуклой оболочки
for (int i = 0; i < pointCount; i++)
{
    convexHullSpline.Points.Add(points[i]);
}

convexHullSpline.IsClosed = true;
convexHullSpline.Color = 16776960; // Желтый цвет

// Создание сплайна, аппроксимирующего кривую Безье
SplineConstruction bezierApproximation = new SplineConstruction(document);

// Определение контрольных точек кривой Безье
FreeNode[] controlPoints = new FreeNode[4];
controlPoints[0] = new FreeNode(document, 40, 40); // Начальная точка
controlPoints[1] = new FreeNode(document, 60, 80); // Первая контрольная точка
controlPoints[2] = new FreeNode(document, 100, 20); // Вторая контрольная точка
controlPoints[3] = new FreeNode(document, 120, 60); // Конечная точка

// Создание точек для аппроксимации кривой Безье
int bezierPoints = 20;
for (int i = 0; i <= bezierPoints; i++)
{
    double t = (double)i / bezierPoints;
    double x = Math.Pow(1 - t, 3) * controlPoints[0].X.Value +
               3 * Math.Pow(1 - t, 2) * t * controlPoints[1].X.Value +
               3 * (1 - t) * Math.Pow(t, 2) * controlPoints[2].X.Value +
               Math.Pow(t, 3) * controlPoints[3].X.Value;
    double y = Math.Pow(1 - t, 3) * controlPoints[0].Y.Value +
               3 * Math.Pow(1 - t, 2) * t * controlPoints[1].Y.Value +
               3 * (1 - t) * Math.Pow(t, 2) * controlPoints[2].Y.Value +
               Math.Pow(t, 3) * controlPoints[3].Y.Value;
    FreeNode point = new FreeNode(document, x, y);
    bezierApproximation.Points.Add(point);
}

bezierApproximation.Color = 65535; // Голубой цвет

// Создание визуальных маркеров контрольных точек
for (int i = 0; i < 4; i++)
{
    CircleConstruction controlMarker = new CircleConstruction(document);
    controlMarker.SetCenterAndRadius(controlPoints[i], 2);
    controlMarker.Color = 16711935; // Пурпурный цвет
    
    // Создание линий между контрольными точками
    if (i > 0)
    {
        LineConstruction controlLine = new LineConstruction(document);
        controlLine.SetTwoNodes(controlPoints[i - 1], controlPoints[i]);
        controlLine.Color = 12632256; // Серый цвет
        controlLine.Style = LineStyle.Dash; // Пунктирная линия
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание сплайнов с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы сплайнов");

// Создание системы сплайнов в форме лепестков
int petalCount = 8;
SplineConstruction[] petalSplines = new SplineConstruction[petalCount];

for (int i = 0; i < petalCount; i++)
{
    petalSplines[i] = new SplineConstruction(document);
    
    double angle = 2 * Math.PI * i / petalCount;
    double centerX = 70;
    double centerY = 70;
    double petalLength = 30;
    int pointsPerPetal = 10;
    
    // Создание точек для лепестка
    for (int j = 0; j <= pointsPerPetal; j++)
    {
        double t = (double)j / pointsPerPetal;
        double radius = petalLength * Math.Sin(Math.PI * t);
        double pointAngle = angle + 0.3 * Math.Sin(Math.PI * t);
        double x = centerX + radius * Math.Cos(pointAngle);
        double y = centerY + radius * Math.Sin(pointAngle);
        FreeNode point = new FreeNode(document, x, y);
        petalSplines[i].Points.Add(point);
    }
    
    // Установка цвета с градиентом
    int intensity = (int)(255 * (double)i / (petalCount - 1));
    petalSplines[i].Color = (intensity << 16) | ((255 - intensity) << 8) | 128;
}

// Создание сплайна в форме звезды
SplineConstruction starSpline = new SplineConstruction(document);

int starPoints = 10;
double outerRadius = 40;
double innerRadius = 20;
double starCenterX = 150;
double starCenterY = 70;

for (int i = 0; i < starPoints; i++)
{
    double radius = (i % 2 == 0) ? outerRadius : innerRadius;
    double angle = 2 * Math.PI * i / starPoints - Math.PI / 2;
    double x = starCenterX + radius * Math.Cos(angle);
    double y = starCenterY + radius * Math.Sin(angle);
    FreeNode point = new FreeNode(document, x, y);
    starSpline.Points.Add(point);
}

starSpline.IsClosed = true;
starSpline.Color = 16711680; // Синий цвет

// Создание сплайна в форме сердца
SplineConstruction heartSpline = new SplineConstruction(document);

int heartPoints = 30;
double heartScale = 15;
double heartCenterX = 70;
double heartCenterY = 130;

for (int i = 0; i <= heartPoints; i++)
{
    double t = 2 * Math.PI * i / heartPoints;
    double x = heartCenterX + heartScale * (16 * Math.Pow(Math.Sin(t), 3)) / 16;
    double y = heartCenterY - heartScale * (13 * Math.Cos(t) - 5 * Math.Cos(2 * t) - 2 * Math.Cos(3 * t) - Math.Cos(4 * t)) / 16;
    FreeNode point = new FreeNode(document, x, y);
    heartSpline.Points.Add(point);
}

heartSpline.IsClosed = true;
heartSpline.Color = 255; // Красный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция сплайнов с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция сплайнов с другими объектами");

// Создание сплайна и связанных объектов
SplineConstruction mainSpline = new SplineConstruction(document);

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
    mainSpline.Points.Add(point);
}

mainSpline.Color = 255; // Красный цвет

// Создание касательных линий в точках сплайна
int tangentCount = 5;
LineConstruction[] tangentLines = new LineConstruction[tangentCount];

for (int i = 0; i < tangentCount; i++)
{
    int pointIndex = i * splinePoints / (tangentCount - 1);
    if (pointIndex >= mainSpline.Points.Count) pointIndex = mainSpline.Points.Count - 1;
    
    FreeNode point = mainSpline.Points[pointIndex];
    
    // Вычисление направления касательной (приблизительно)
    double tangentLength = 10;
    double tangentAngle = Math.PI / 4 * Math.Sin(2 * Math.PI * i / (tangentCount - 1));
    double endX = point.X.Value + tangentLength * Math.Cos(tangentAngle);
    double endY = point.Y.Value + tangentLength * Math.Sin(tangentAngle);
    
    FreeNode endPoint = new FreeNode(document, endX, endY);
    tangentLines[i] = new LineConstruction(document);
    tangentLines[i].SetTwoNodes(point, endPoint);
    tangentLines[i].Color = 65280; // Зеленый цвет
}

// Создание нормалей к сплайну
int normalCount = 5;
LineConstruction[] normalLines = new LineConstruction[normalCount];

for (int i = 0; i < normalCount; i++)
{
    int pointIndex = i * splinePoints / (normalCount - 1);
    if (pointIndex >= mainSpline.Points.Count) pointIndex = mainSpline.Points.Count - 1;
    
    FreeNode point = mainSpline.Points[pointIndex];
    
    // Вычисление направления нормали (перпендикулярно касательной)
    double normalLength = 8;
    double normalAngle = Math.PI / 4 * Math.Sin(2 * Math.PI * i / (normalCount - 1)) + Math.PI / 2;
    double endX = point.X.Value + normalLength * Math.Cos(normalAngle);
    double endY = point.Y.Value + normalLength * Math.Sin(normalAngle);
    
    FreeNode endPoint = new FreeNode(document, endX, endY);
    normalLines[i] = new LineConstruction(document);
    normalLines[i].SetTwoNodes(point, endPoint);
    normalLines[i].Color = 16711680; // Синий цвет
}

// Создание окружностей в точках сплайна
int circleCount = 8;
CircleConstruction[] pointCircles = new CircleConstruction[circleCount];

for (int i = 0; i < circleCount; i++)
{
    int pointIndex = i * mainSpline.Points.Count / (circleCount - 1);
    if (pointIndex >= mainSpline.Points.Count) pointIndex = mainSpline.Points.Count - 1;
    
    FreeNode point = mainSpline.Points[pointIndex];
    pointCircles[i] = new CircleConstruction(document);
    pointCircles[i].SetCenterAndRadius(point, 2);
    pointCircles[i].Color = 16776960; // Желтый цвет
}

// Создание огибающей сплайна
SplineConstruction envelopeSpline = new SplineConstruction(document);

// Создание точек огибающей (приблизительно)
for (int i = 0; i <= splinePoints; i++)
{
    double t = (double)i / splinePoints;
    double x = startX + t * 100;
    double y = startY + 30 * Math.Sin(Math.PI * t) + 15;
    FreeNode point = new FreeNode(document, x, y);
    envelopeSpline.Points.Add(point);
}

envelopeSpline.Color = 16711935; // Пурпурный цвет
envelopeSpline.Style = LineStyle.Dash; // Пунктирная линия

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством сплайнов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества сплайнов с минимальными вызовами API
int splineCount = 50;
SplineConstruction[] splines = new SplineConstruction[splineCount];

// Предварительное создание точек
int pointsPerSpline = 8;
FreeNode[,] allPoints = new FreeNode[splineCount, pointsPerSpline];

Random random = new Random();
for (int i = 0; i < splineCount; i++)
{
    double baseX = 20 + random.NextDouble() * 160;
    double baseY = 20 + random.NextDouble() * 110;
    
    for (int j = 0; j < pointsPerSpline; j++)
    {
        double x = baseX + (j - pointsPerSpline/2) * 5 + random.NextDouble() * 4 - 2;
        double y = baseY + (random.NextDouble() - 0.5) * 20;
        allPoints[i, j] = new FreeNode(document, x, y);
    }
}

// Создание сплайнов
for (int i = 0; i < splineCount; i++)
{
    splines[i] = new SplineConstruction(document);
    
    for (int j = 0; j < pointsPerSpline; j++)
    {
        splines[i].Points.Add(allPoints[i, j]);
    }
    
    // Установка цвета
    int red = (int)(255 * random.NextDouble());
    int green = (int)(255 * random.NextDouble());
    int blue = (int)(255 * random.NextDouble());
    splines[i].Color = (red << 16) | (green << 8) | blue;
    
    // Установка толщины линии
    splines[i].LineWidth = 1 + (int)(random.NextDouble() * 2);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими сплайнами и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические сплайны");

// Создание сплайна с возможностью динамического обновления
SplineConstruction dynamicSpline = new SplineConstruction(document);

// Создание начальных точек
int dynamicPoints = 10;
FreeNode[] dynamicNodes = new FreeNode[dynamicPoints];

for (int i = 0; i < dynamicPoints; i++)
{
    double x = 30 + i * 10;
    double y = 50 + 20 * Math.Sin(i * Math.PI / (dynamicPoints - 1));
    dynamicNodes[i] = new FreeNode(document, x, y);
    dynamicSpline.Points.Add(dynamicNodes[i]);
}

dynamicSpline.Color = 255; // Красный цвет

// Создание сплайна, который будет менять свою форму
SplineConstruction morphingSpline = new SplineConstruction(document);

int morphingPoints = 12;
FreeNode[] morphingNodes = new FreeNode[morphingPoints];

for (int i = 0; i < morphingPoints; i++)
{
    double x = 50 + i * 8;
    double y = 100;
    morphingNodes[i] = new FreeNode(document, x, y);
    morphingSpline.Points.Add(morphingNodes[i]);
}

morphingSpline.Color = 65280; // Зеленый цвет

// Создание системы сплайнов с анимацией
int animatedSplineCount = 5;
SplineConstruction[] animatedSplines = new SplineConstruction[animatedSplineCount];
FreeNode[,][] animatedNodes = new FreeNode[animatedSplineCount, 8][];

for (int i = 0; i < animatedSplineCount; i++)
{
    animatedSplines[i] = new SplineConstruction(document);
    animatedNodes[i] = new FreeNode[8][];
    
    for (int j = 0; j < 8; j++)
    {
        double baseX = 120 + i * 25;
        double baseY = 30 + j * 15;
        animatedNodes[i][j] = new FreeNode(document, baseX, baseY);
        animatedSplines[i].Points.Add(animatedNodes[i][j]);
    }
    
    animatedSplines[i].Color = 16711680; // Синий цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств сплайнов
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicSplines(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических сплайнов");
    
    // Обновление точек динамического сплайна
    for (int i = 0; i < dynamicPoints; i++)
    {
        double y = 50 + 20 * Math.Sin(i * Math.PI / (dynamicPoints - 1) + time * 0.5);
        dynamicNodes[i].Y.Value = y;
    }
    
    // Обновление точек морфирующего сплайна
    for (int i = 0; i < morphingPoints; i++)
    {
        double y = 100 + 15 * Math.Sin(time * 0.3 + i * Math.PI / (morphingPoints - 1));
        morphingNodes[i].Y.Value = y;
    }
    
    // Обновление анимированных сплайнов
    for (int i = 0; i < animatedSplineCount; i++)
    {
        for (int j = 0; j < 8; j++)
        {
            double x = 120 + i * 25 + 5 * Math.Sin(time * 0.5 + i + j);
            double y = 30 + j * 15 + 3 * Math.Cos(time * 0.7 + i + j);
            animatedNodes[i][j].X.Value = x;
            animatedNodes[i][j].Y.Value = y;
        }
        
        // Изменение цвета в зависимости от времени
        int red = (int)(255 * (1 + Math.Sin(time * 0.5 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.5 + i + 1)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.5 + i + 2)) / 2);
        animatedSplines[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
```

## Свойства и методы

### Основные свойства:

- `Points` - Коллекция точек сплайна
- `IsClosed` - Является ли сплайн замкнутым
- `SplineType` - Тип сплайна
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

### Основные методы:

- `AddPoint` - Добавление точки к сплайну
- `RemovePoint` - Удаление точки из сплайна
- `InsertPoint` - Вставка точки в сплайн
- `ClearPoints` - Очистка всех точек сплайна

## Заключение

Продвинутое использование класса `SplineConstruction` включает в себя создание сложных кривых, параметризованных конструкций, работу с массивами сплайнов, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами сплайнов важно учитывать производительность и использовать эффективные алгоритмы для вычисления координат и установления связей между объектами.
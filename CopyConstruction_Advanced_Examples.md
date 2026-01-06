# CopyConstruction - продвинутые примеры использования

Класс `CopyConstruction` представляет линию построения, полученную ассоциативным копированием в T-Flex CAD API. Этот класс предоставляет возможности для создания копий объектов с различными преобразованиями.

## Продвинутые примеры использования

### 1. Создание сложных массивов копий

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сложных массивов копий");

// Создание исходного объекта (звезды)
PathConstruction sourceStar = new PathConstruction(document);

int starPoints = 5;
double outerRadius = 10;
double innerRadius = 5;
double centerX = 30;
double centerY = 30;

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

// Создание двумерного массива копий
int rows = 5;
int cols = 6;
double spacingX = 25;
double spacingY = 20;

CopyConstruction[,] starCopies = new CopyConstruction[rows, cols];

for (int i = 0; i < rows; i++)
{
    for (int j = 0; j < cols; j++)
    {
        starCopies[i, j] = new CopyConstruction(document);
        starCopies[i, j].Source = sourceStar;
        
        // Создание матрицы преобразования
        Matrix2D transform = new Matrix2D();
        transform.Translate(j * spacingX, i * spacingY);
        
        // Добавление поворота для каждой копии
        double rotationAngle = (i + j) * Math.PI / 12; // 15 градусов * (i + j)
        transform.Rotate(rotationAngle);
        
        starCopies[i, j].Transformation = transform;
        
        // Установка цвета с градиентом
        int red = (int)(255 * (double)i / (rows - 1));
        int green = (int)(255 * (double)j / (cols - 1));
        int blue = 255 - (red + green) / 2;
        starCopies[i, j].Color = (red << 16) | (green << 8) | blue;
    }
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание копий с геометрическими преобразованиями

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание копий с геометрическими преобразованиями");

// Создание исходного объекта (эллипса)
EllipseConstruction sourceEllipse = new EllipseConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
FreeNode majorNode = new FreeNode(document, 70, 50);
FreeNode minorNode = new FreeNode(document, 50, 65);
sourceEllipse.SetCenterAndTwoNodes(center, majorNode, minorNode);
sourceEllipse.Color = 255; // Красный цвет

// Создание копий с различными преобразованиями
int copyCount = 12;
CopyConstruction[] ellipseCopies = new CopyConstruction[copyCount];

for (int i = 0; i < copyCount; i++)
{
    ellipseCopies[i] = new CopyConstruction(document);
    ellipseCopies[i].Source = sourceEllipse;
    
    // Создание сложной матрицы преобразования
    Matrix2D transform = new Matrix2D();
    
    // Перемещение
    double offsetX = 80 * Math.Cos(2 * Math.PI * i / copyCount);
    double offsetY = 80 * Math.Sin(2 * Math.PI * i / copyCount);
    transform.Translate(offsetX, offsetY);
    
    // Поворот
    double rotationAngle = 2 * Math.PI * i / copyCount;
    transform.Rotate(rotationAngle);
    
    // Масштабирование
    double scale = 0.5 + 0.5 * Math.Sin(2 * Math.PI * i / copyCount);
    transform.Scale(scale, scale);
    
    // Сдвиг (skew)
    double skewAngle = Math.PI * i / copyCount;
    transform.Skew(skewAngle);
    
    ellipseCopies[i].Transformation = transform;
    
    // Установка цвета
    int red = (int)(255 * (1 + Math.Sin(2 * Math.PI * i / copyCount)) / 2);
    int green = (int)(255 * (1 + Math.Cos(2 * Math.PI * i / copyCount + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(2 * Math.PI * i / copyCount + 2 * Math.PI / 3)) / 2);
    ellipseCopies[i].Color = (red << 16) | (green << 8) | blue;
}

// Создание копий с отражением
CopyConstruction[] mirroredCopies = new CopyConstruction[4];

for (int i = 0; i < 4; i++)
{
    mirroredCopies[i] = new CopyConstruction(document);
    mirroredCopies[i].Source = sourceEllipse;
    
    Matrix2D transform = new Matrix2D();
    transform.Translate(0, 40 * i);
    
    // Отражение по горизонтали или вертикали
    if (i % 2 == 0)
    {
        transform.Scale(-1, 1); // Отражение по горизонтали
    }
    else
    {
        transform.Scale(1, -1); // Отражение по вертикали
    }
    
    mirroredCopies[i].Transformation = transform;
    mirroredCopies[i].Color = 65280; // Зеленый цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание копий с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы копий");

// Создание исходного объекта (сплайна в форме волны)
SplineConstruction sourceWave = new SplineConstruction(document);

int wavePoints = 20;
double amplitude = 10;
double wavelength = 5;
double startX = 20;
double startY = 30;

for (int i = 0; i <= wavePoints; i++)
{
    double x = startX + i * 3;
    double y = startY + amplitude * Math.Sin(i * 2 * Math.PI / wavelength);
    FreeNode point = new FreeNode(document, x, y);
    sourceWave.Points.Add(point);
}

sourceWave.Color = 255; // Красный цвет

// Создание параметризованной системы копий
int paramRows = 6;
int paramCols = 8;
CopyConstruction[,] waveCopies = new CopyConstruction[paramRows, paramCols];

for (int i = 0; i < paramRows; i++)
{
    for (int j = 0; j < paramCols; j++)
    {
        waveCopies[i, j] = new CopyConstruction(document);
        waveCopies[i, j].Source = sourceWave;
        
        Matrix2D transform = new Matrix2D();
        
        // Параметрическое перемещение
        double offsetX = j * 20;
        double offsetY = i * 25 + 60;
        transform.Translate(offsetX, offsetY);
        
        // Параметрическое масштабирование
        double scale = 0.5 + 0.5 * (double)j / (paramCols - 1);
        transform.Scale(scale, scale);
        
        // Параметрический поворот
        double rotation = Math.PI * (double)i / (paramRows - 1);
        transform.Rotate(rotation);
        
        waveCopies[i, j].Transformation = transform;
        
        // Установка цвета в зависимости от параметров
        int red = (int)(255 * (double)i / (paramRows - 1));
        int green = (int)(255 * (double)j / (paramCols - 1));
        int blue = 255 - (red + green) / 2;
        waveCopies[i, j].Color = (red << 16) | (green << 8) | blue;
        
        // Установка толщины линии
        waveCopies[i, j].LineWidth = 1 + (int)((double)i / (paramRows - 1) * 3);
    }
}

// Создание копий с изменяющейся амплитудой
int amplitudeCopies = 10;
CopyConstruction[] amplitudeVariations = new CopyConstruction[amplitudeCopies];

for (int i = 0; i < amplitudeCopies; i++)
{
    amplitudeVariations[i] = new CopyConstruction(document);
    amplitudeVariations[i].Source = sourceWave;
    
    Matrix2D transform = new Matrix2D();
    transform.Translate(0, i * 15 + 250);
    
    // Масштабирование по вертикали для изменения амплитуды
    double amplitudeScale = 0.5 + 1.5 * (double)i / (amplitudeCopies - 1);
    transform.Scale(1, amplitudeScale);
    
    amplitudeVariations[i].Transformation = transform;
    amplitudeVariations[i].Color = 16711680; // Синий цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция копий с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция копий с другими объектами");

// Создание исходного объекта (окружности)
CircleConstruction sourceCircle = new CircleConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
sourceCircle.SetCenterAndRadius(center, 15);
sourceCircle.Color = 255; // Красный цвет

// Создание копий, интегрированных с линиями
int integratedCopies = 8;
CopyConstruction[] integratedCopiesArray = new CopyConstruction[integratedCopies];
LineConstruction[] connectionLines = new LineConstruction[integratedCopies];

for (int i = 0; i < integratedCopies; i++)
{
    integratedCopiesArray[i] = new CopyConstruction(document);
    integratedCopiesArray[i].Source = sourceCircle;
    
    Matrix2D transform = new Matrix2D();
    double angle = 2 * Math.PI * i / integratedCopies;
    double radius = 50;
    double offsetX = radius * Math.Cos(angle);
    double offsetY = radius * Math.Sin(angle);
    transform.Translate(offsetX, offsetY);
    integratedCopiesArray[i].Transformation = transform;
    integratedCopiesArray[i].Color = 65280; // Зеленый цвет
    
    // Создание соединительных линий
    double copyCenterX = center.X.Value + offsetX;
    double copyCenterY = center.Y.Value + offsetY;
    FreeNode copyCenter = new FreeNode(document, copyCenterX, copyCenterY);
    connectionLines[i] = new LineConstruction(document);
    connectionLines[i].SetTwoNodes(center, copyCenter);
    connectionLines[i].Color = 12632256; // Серый цвет
    connectionLines[i].Style = LineStyle.Dash; // Пунктирная линия
}

// Создание копий, интегрированных с контурами
PathConstruction referencePath = new PathConstruction(document);

// Создание контура в форме квадрата
FreeNode[] squareNodes = new FreeNode[4];
squareNodes[0] = new FreeNode(document, 120, 30);
squareNodes[1] = new FreeNode(document, 170, 30);
squareNodes[2] = new FreeNode(document, 170, 80);
squareNodes[3] = new FreeNode(document, 120, 80);

for (int i = 0; i < 4; i++)
{
    referencePath.AddSegment(squareNodes[i], squareNodes[(i + 1) % 4]);
}

referencePath.Color = 16711680; // Синий цвет

// Создание копий вдоль контура
int pathCopies = 12;
CopyConstruction[] pathCopiesArray = new CopyConstruction[pathCopies];

for (int i = 0; i < pathCopies; i++)
{
    pathCopiesArray[i] = new CopyConstruction(document);
    pathCopiesArray[i].Source = sourceCircle;
    
    Matrix2D transform = new Matrix2D();
    
    // Вычисление позиции вдоль контура (приблизительно)
    double t = (double)i / (pathCopies - 1);
    int segmentIndex = (int)(t * 4);
    double segmentT = (t * 4) - segmentIndex;
    
    double x = squareNodes[segmentIndex].X.Value + 
              segmentT * (squareNodes[(segmentIndex + 1) % 4].X.Value - squareNodes[segmentIndex].X.Value);
    double y = squareNodes[segmentIndex].Y.Value + 
              segmentT * (squareNodes[(segmentIndex + 1) % 4].Y.Value - squareNodes[segmentIndex].Y.Value);
    
    transform.Translate(x - center.X.Value, y - center.Y.Value);
    
    // Добавление поворота в зависимости от позиции
    double rotation = 2 * Math.PI * i / pathCopies;
    transform.Rotate(rotation);
    
    pathCopiesArray[i].Transformation = transform;
    pathCopiesArray[i].Color = 16776960; // Желтый цвет
}

// Создание копий, интегрированных с другими копиями
CopyConstruction[] secondaryCopies = new CopyConstruction[integratedCopies];

for (int i = 0; i < integratedCopies; i++)
{
    secondaryCopies[i] = new CopyConstruction(document);
    secondaryCopies[i].Source = integratedCopiesArray[i]; // Копия копии
    
    Matrix2D transform = new Matrix2D();
    transform.Translate(20 * Math.Cos(i * Math.PI / 4), 20 * Math.Sin(i * Math.PI / 4));
    transform.Scale(0.7, 0.7);
    secondaryCopies[i].Transformation = transform;
    secondaryCopies[i].Color = 16711935; // Пурпурный цвет
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством копий

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества копий с минимальными вызовами API
int copyCount = 200;
CopyConstruction[] copies = new CopyConstruction[copyCount];

// Создание исходного объекта (простой линии)
LineConstruction sourceLine = new LineConstruction(document);
FreeNode startNode = new FreeNode(document, 0, 0);
FreeNode endNode = new FreeNode(document, 10, 0);
sourceLine.SetTwoNodes(startNode, endNode);

// Предварительное создание матриц преобразования
Matrix2D[] transforms = new Matrix2D[copyCount];

Random random = new Random();
for (int i = 0; i < copyCount; i++)
{
    transforms[i] = new Matrix2D();
    
    // Случайное перемещение
    double offsetX = 20 + random.NextDouble() * 160;
    double offsetY = 20 + random.NextDouble() * 110;
    transforms[i].Translate(offsetX, offsetY);
    
    // Случайный поворот
    double rotation = random.NextDouble() * 2 * Math.PI;
    transforms[i].Rotate(rotation);
    
    // Случайное масштабирование
    double scale = 0.5 + random.NextDouble() * 1.5;
    transforms[i].Scale(scale, scale);
}

// Создание копий
for (int i = 0; i < copyCount; i++)
{
    copies[i] = new CopyConstruction(document);
    copies[i].Source = sourceLine;
    copies[i].Transformation = transforms[i];
    
    // Установка цвета
    int red = (int)(255 * random.NextDouble());
    int green = (int)(255 * random.NextDouble());
    int blue = (int)(255 * random.NextDouble());
    copies[i].Color = (red << 16) | (green << 8) | blue;
    
    // Установка толщины линии
    copies[i].LineWidth = 1 + (int)(random.NextDouble() * 3);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими копиями и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические копии");

// Создание исходного объекта с возможностью динамического обновления
CircleConstruction dynamicSource = new CircleConstruction(document);
FreeNode dynamicCenter = new FreeNode(document, 50, 50);
dynamicSource.SetCenterAndRadius(dynamicCenter, 10);
dynamicSource.Color = 255; // Красный цвет

// Создание копий с возможностью динамического обновления
int dynamicCopyCount = 8;
CopyConstruction[] dynamicCopies = new CopyConstruction[dynamicCopyCount];
Matrix2D[] baseTransforms = new Matrix2D[dynamicCopyCount];

for (int i = 0; i < dynamicCopyCount; i++)
{
    dynamicCopies[i] = new CopyConstruction(document);
    dynamicCopies[i].Source = dynamicSource;
    
    // Сохранение базовой матрицы преобразования
    baseTransforms[i] = new Matrix2D();
    double angle = 2 * Math.PI * i / dynamicCopyCount;
    double radius = 40;
    baseTransforms[i].Translate(radius * Math.Cos(angle), radius * Math.Sin(angle));
    
    dynamicCopies[i].Transformation = baseTransforms[i];
    dynamicCopies[i].Color = 65280; // Зеленый цвет
}

// Создание копий, которые будут менять свои параметры
CopyConstruction[] morphingCopies = new CopyConstruction[6];
Matrix2D[] morphingBaseTransforms = new Matrix2D[6];

for (int i = 0; i < 6; i++)
{
    morphingCopies[i] = new CopyConstruction(document);
    morphingCopies[i].Source = dynamicSource;
    
    morphingBaseTransforms[i] = new Matrix2D();
    morphingBaseTransforms[i].Translate(100 + i * 20, 50);
    
    morphingCopies[i].Transformation = morphingBaseTransforms[i];
    morphingCopies[i].Color = 16711680; // Синий цвет
}

// Создание системы копий с анимацией
int animatedCopyCount = 12;
CopyConstruction[] animatedCopies = new CopyConstruction[animatedCopyCount];
Matrix2D[] animatedBaseTransforms = new Matrix2D[animatedCopyCount];

for (int i = 0; i < animatedCopyCount; i++)
{
    animatedCopies[i] = new CopyConstruction(document);
    animatedCopies[i].Source = dynamicSource;
    
    animatedBaseTransforms[i] = new Matrix2D();
    double angle = 2 * Math.PI * i / animatedCopyCount;
    double radius = 70;
    animatedBaseTransforms[i].Translate(150 + radius * Math.Cos(angle), 50 + radius * Math.Sin(angle));
    
    animatedCopies[i].Transformation = animatedBaseTransforms[i];
    animatedCopies[i].Color = 16776960; // Желтый цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств копий
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicCopies(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических копий");
    
    // Обновление центра исходного объекта
    double newX = 50 + 10 * Math.Sin(time * 0.5);
    double newY = 50 + 10 * Math.Cos(time * 0.5);
    dynamicCenter.X.Value = newX;
    dynamicCenter.Y.Value = newY;
    
    // Обновление преобразований динамических копий
    for (int i = 0; i < dynamicCopyCount; i++)
    {
        Matrix2D newTransform = new Matrix2D(baseTransforms[i]);
        double rotation = time * 0.3 + i * Math.PI / 4;
        newTransform.Rotate(rotation);
        dynamicCopies[i].Transformation = newTransform;
    }
    
    // Обновление преобразований морфирующих копий
    for (int i = 0; i < 6; i++)
    {
        Matrix2D newTransform = new Matrix2D(morphingBaseTransforms[i]);
        double scale = 0.8 + 0.4 * Math.Sin(time * 0.7 + i);
        newTransform.Scale(scale, scale);
        morphingCopies[i].Transformation = newTransform;
        
        // Изменение цвета
        int red = (int)(255 * (1 + Math.Sin(time * 0.7 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.7 + i + Math.PI / 3)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.7 + i + 2 * Math.PI / 3)) / 2);
        morphingCopies[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Обновление анимированных копий
    for (int i = 0; i < animatedCopyCount; i++)
    {
        Matrix2D newTransform = new Matrix2D(animatedBaseTransforms[i]);
        double offsetX = 5 * Math.Sin(time * 0.5 + i);
        double offsetY = 5 * Math.Cos(time * 0.5 + i);
        newTransform.Translate(offsetX, offsetY);
        animatedCopies[i].Transformation = newTransform;
        
        // Изменение цвета в зависимости от времени
        int red = (int)(255 * (1 + Math.Sin(time * 0.3 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.3 + i + 1)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.3 + i + 2)) / 2);
        animatedCopies[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
```

## Свойства и методы

### Основные свойства:

- `Source` - Исходная линия построения
- `SourceCopyOperation` - Исходный объект-копия
- `Transformation` - Преобразование
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
- `SetTransformation` - Установка преобразования
- `GetTransformedGeometry` - Получение преобразованной геометрии

## Заключение

Продвинутое использование класса `CopyConstruction` включает в себя создание сложных массивов копий, применение различных геометрических преобразований, параметризованные конструкции, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами копий важно учитывать производительность и использовать эффективные алгоритмы для вычисления преобразований и установления связей между объектами.
# SymmetryConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
SymmetryConstruction представляет собой симметричную линию построения в T-Flex CAD API. Это геометрический элемент для создания симметричных копий других геометрических объектов относительно заданной оси.

## Основные свойства
- `Source` - Исходная линия построения (Construction)
- `Axis` - Ось симметрии (LineConstruction)
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Конструкторы
```csharp
// Создание пустой симметричной линии построения
SymmetryConstruction symmetry = new SymmetryConstruction(document);
```

## Основные методы
- `SetSource(Construction source)` - Установка исходного объекта
- `SetAxis(LineConstruction axis)` - Установка оси симметрии
- `GetSymmetricGeometry()` - Получение симметричной геометрии
- `GetReflectionMatrix()` - Получение матрицы отражения

## Примеры использования

### Базовое использование
```csharp
// Создание простой симметрии
LineConstruction originalLine = new LineConstruction(document);
originalLine.SetTwoNodes(new FreeNode(document, 30, 40), new FreeNode(document, 50, 60));

// Создание оси симметрии (вертикальная линия)
LineConstruction symmetryAxis = new LineConstruction(document);
symmetryAxis.SetTwoNodes(new FreeNode(document, 40, 30), new FreeNode(document, 40, 70));

SymmetryConstruction symmetry = new SymmetryConstruction(document);
symmetry.SetSource(originalLine);
symmetry.SetAxis(symmetryAxis);
symmetry.Color = 255; // Красный цвет
```

### Создание симметрии контура
```csharp
// Создание симметрии замкнутого контура
PathConstruction originalPath = new PathConstruction(document);

// Создание треугольного контура
FreeNode[] nodes = new FreeNode[3];
nodes[0] = new FreeNode(document, 30, 30);
nodes[1] = new FreeNode(document, 50, 30);
nodes[2] = new FreeNode(document, 40, 50);

for (int i = 0; i < 3; i++)
{
    originalPath.AddSegment(nodes[i], nodes[(i + 1) % 3]);
}

// Создание оси симметрии (вертикальная линия через центр)
LineConstruction symmetryAxis = new LineConstruction(document);
symmetryAxis.SetTwoNodes(new FreeNode(document, 40, 20), new FreeNode(document, 40, 60));

SymmetryConstruction pathSymmetry = new SymmetryConstruction(document);
pathSymmetry.SetSource(originalPath);
pathSymmetry.SetAxis(symmetryAxis);
pathSymmetry.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание множественных симметрий
```csharp
// Создание множественных симметрий
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 30, 50), 10);

int symmetryCount = 4;
SymmetryConstruction[] symmetries = new SymmetryConstruction[symmetryCount];
LineConstruction[] symmetryAxes = new LineConstruction[symmetryCount];

for (int i = 0; i < symmetryCount; i++)
{
    symmetries[i] = new SymmetryConstruction(document);
    symmetries[i].SetSource(originalCircle);
    
    // Создание осей симметрии под разными углами
    double angle = Math.PI * i / symmetryCount;
    double axisStartX = 50 - 30 * Math.Cos(angle);
    double axisStartY = 50 - 30 * Math.Sin(angle);
    double axisEndX = 50 + 30 * Math.Cos(angle);
    double axisEndY = 50 + 30 * Math.Sin(angle);
    
    FreeNode axisStart = new FreeNode(document, axisStartX, axisStartY);
    FreeNode axisEnd = new FreeNode(document, axisEndX, axisEndY);
    symmetryAxes[i] = new LineConstruction(document);
    symmetryAxes[i].SetTwoNodes(axisStart, axisEnd);
    symmetryAxes[i].Color = 12632256; // Серый цвет
    symmetryAxes[i].Style = LineStyle.Dash;
    
    symmetries[i].SetAxis(symmetryAxes[i]);
    
    // Установка цвета с градиентом
    int red = (int)(255 * (double)i / (symmetryCount - 1));
    int green = 255 - red;
    int blue = 128;
    symmetries[i].Color = (red << 16) | (green << 8) | blue;
}
```

### Создание симметрий с геометрическими расчетами
```csharp
// Создание симметрий с геометрическими расчетами
SplineConstruction originalSpline = new SplineConstruction(document);

// Создание точек сплайна в форме волны
int pointCount = 8;
for (int i = 0; i < pointCount; i++)
{
    double x = 20 + i * 5;
    double y = 50 + 10 * Math.Sin(i * 0.5);
    FreeNode point = new FreeNode(document, x, y);
    originalSpline.Points.Add(point);
}

// Создание симметрии относительно горизонтальной оси
LineConstruction horizontalAxis = new LineConstruction(document);
horizontalAxis.SetTwoNodes(new FreeNode(document, 20, 50), new FreeNode(document, 60, 50));

SymmetryConstruction splineSymmetry = new SymmetryConstruction(document);
splineSymmetry.SetSource(originalSpline);
splineSymmetry.SetAxis(horizontalAxis);
splineSymmetry.Color = 16711680; // Синий цвет
```

## Связанные объекты
- CopyConstruction - Копия линии построения
- OffsetConstruction - Смещенная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- LineConstruction - Линия построения
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества симметрий
2. Убедитесь, что исходные объекты и оси симметрии существуют и корректны
3. Проверяйте геометрические свойства симметрий перед использованием в сложных расчетах

## Лучшие практики
1. Используйте параметризованные симметрии для создания динамических конструкций
2. При создании больших массивов симметрий используйте оптимизацию производительности
3. Используйте симметрии повторно при создании сложных конструкций
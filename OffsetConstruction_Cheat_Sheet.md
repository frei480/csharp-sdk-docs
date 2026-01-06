# OffsetConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
OffsetConstruction представляет собой смещенную линию построения в T-Flex CAD API. Это геометрический элемент для создания параллельных копий других геометрических объектов на заданном расстоянии.

## Основные свойства
- `Source` - Исходная линия построения (Construction)
- `Distance` - Расстояние смещения (DoubleParameter)
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
// Создание пустой смещенной линии построения
OffsetConstruction offset = new OffsetConstruction(document);
```

## Основные методы
- `SetSource(Construction source)` - Установка исходного объекта
- `SetDistance(double distance)` - Установка расстояния смещения
- `GetOffsetGeometry()` - Получение смещенной геометрии
- `GetNormalVectorAtPoint(Node point)` - Получение вектора нормали в точке

## Примеры использования

### Базовое использование
```csharp
// Создание простого смещения линии
LineConstruction originalLine = new LineConstruction(document);
originalLine.SetTwoNodes(new FreeNode(document, 30, 50), new FreeNode(document, 70, 50));

OffsetConstruction offset = new OffsetConstruction(document);
offset.SetSource(originalLine);
offset.SetDistance(10); // Смещение на 10 единиц вверх
offset.Color = 255; // Красный цвет
```

### Создание смещения контура
```csharp
// Создание смещения замкнутого контура
PathConstruction originalPath = new PathConstruction(document);

// Создание прямоугольного контура
FreeNode[] nodes = new FreeNode[4];
nodes[0] = new FreeNode(document, 40, 40);
nodes[1] = new FreeNode(document, 60, 40);
nodes[2] = new FreeNode(document, 60, 60);
nodes[3] = new FreeNode(document, 40, 60);

for (int i = 0; i < 4; i++)
{
    originalPath.AddSegment(nodes[i], nodes[(i + 1) % 4]);
}

OffsetConstruction pathOffset = new OffsetConstruction(document);
pathOffset.SetSource(originalPath);
pathOffset.SetDistance(5); // Смещение на 5 единиц внутрь
pathOffset.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание множественных смещений
```csharp
// Создание множественных смещений
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 50, 50), 20);

int offsetCount = 5;
double baseDistance = 5;
OffsetConstruction[] offsets = new OffsetConstruction[offsetCount];

for (int i = 0; i < offsetCount; i++)
{
    offsets[i] = new OffsetConstruction(document);
    offsets[i].SetSource(originalCircle);
    offsets[i].SetDistance(baseDistance * (i + 1));
    
    // Установка цвета с градиентом
    int red = (int)(255 * (double)i / (offsetCount - 1));
    int green = 255 - red;
    int blue = 128;
    offsets[i].Color = (red << 16) | (green << 8) | blue;
    offsets[i].Style = LineStyle.Dash;
}
```

### Создание смещений с геометрическими расчетами
```csharp
// Создание смещений с геометрическими расчетами
SplineConstruction originalSpline = new SplineConstruction(document);

// Создание точек сплайна в форме волны
int pointCount = 10;
for (int i = 0; i < pointCount; i++)
{
    double x = 20 + i * 8;
    double y = 50 + 15 * Math.Sin(i * 0.5);
    FreeNode point = new FreeNode(document, x, y);
    originalSpline.Points.Add(point);
}

// Создание смещений в обе стороны
OffsetConstruction[] splineOffsets = new OffsetConstruction[2];
double[] distances = { 5, -5 }; // В обе стороны от сплайна

for (int i = 0; i < 2; i++)
{
    splineOffsets[i] = new OffsetConstruction(document);
    splineOffsets[i].SetSource(originalSpline);
    splineOffsets[i].SetDistance(distances[i]);
    splineOffsets[i].Color = (i == 0) ? 255 : 16711680; // Красный и синий
    splineOffsets[i].Style = LineStyle.Dash;
}
```

## Связанные объекты
- CopyConstruction - Копия линии построения
- SymmetryConstruction - Симметричная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества смещений
2. Убедитесь, что исходные объекты существуют и корректны
3. Проверяйте допустимые значения расстояний смещения

## Лучшие практики
1. Используйте параметризованные смещения для создания динамических конструкций
2. При создании больших массивов смещений используйте оптимизацию производительности
3. Используйте смещения повторно при создании сложных конструкций
# SplineConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
SplineConstruction представляет собой сплайн построения в T-Flex CAD API. Это геометрический элемент для создания гладких кривых, проходящих через заданные точки.

## Основные свойства
- `Points` - Коллекция точек сплайна (NodeCollection)
- `IsClosed` - Является ли сплайн замкнутым (bool)
- `GeometryType` - Тип геометрии сплайна построения
- `SubType` - Подтип сплайна построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Конструкторы
```csharp
// Создание пустого сплайна построения
SplineConstruction spline = new SplineConstruction(document);
```

## Основные методы
- `AddPoint(Node point)` - Добавление точки в сплайн
- `RemovePoint(Node point)` - Удаление точки из сплайна
- `ClearPoints()` - Очистка всех точек сплайна
- `GetLength()` - Получение длины сплайна
- `GetPointAtParameter(double parameter)` - Получение точки на сплайне по параметру
- `GetTangentAtParameter(double parameter)` - Получение касательной в точке сплайна по параметру
- `IsPointOnSpline(Node point, double tolerance)` - Проверка, находится ли точка на сплайне с заданной точностью

## Примеры использования

### Базовое использование
```csharp
// Создание сплайна через заданные точки
SplineConstruction spline = new SplineConstruction(document);

// Добавление точек
FreeNode point1 = new FreeNode(document, 20, 30);
FreeNode point2 = new FreeNode(document, 40, 50);
FreeNode point3 = new FreeNode(document, 60, 40);
FreeNode point4 = new FreeNode(document, 80, 60);

spline.Points.Add(point1);
spline.Points.Add(point2);
spline.Points.Add(point3);
spline.Points.Add(point4);

spline.Color = 255; // Красный цвет
```

### Создание замкнутого сплайна
```csharp
// Создание замкнутого сплайна
SplineConstruction closedSpline = new SplineConstruction(document);
closedSpline.IsClosed = true;

// Добавление точек для создания замкнутой формы
FreeNode[] points = new FreeNode[5];
points[0] = new FreeNode(document, 50, 30);
points[1] = new FreeNode(document, 70, 40);
points[2] = new FreeNode(document, 60, 60);
points[3] = new FreeNode(document, 40, 60);
points[4] = new FreeNode(document, 30, 40);

for (int i = 0; i < 5; i++)
{
    closedSpline.Points.Add(points[i]);
}

closedSpline.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание сложных сплайнов
```csharp
// Создание сложного сплайна с множеством точек
SplineConstruction complexSpline = new SplineConstruction(document);

// Создание точек в форме синусоиды
int pointCount = 20;
double startX = 20;
double startY = 50;
double amplitude = 20;
double frequency = 0.5;

for (int i = 0; i < pointCount; i++)
{
    double x = startX + i * 5;
    double y = startY + amplitude * Math.Sin(i * frequency);
    FreeNode point = new FreeNode(document, x, y);
    complexSpline.Points.Add(point);
}

complexSpline.Color = 16711680; // Синий цвет
complexSpline.LineWidth = 2;
```

### Создание сплайнов с геометрическими расчетами
```csharp
// Создание сплайна на основе геометрических расчетов
SplineConstruction calculatedSpline = new SplineConstruction(document);

// Создание точек в форме спирали
int spiralPoints = 30;
double centerX = 50;
double centerY = 50;
double radiusIncrement = 2;

for (int i = 0; i < spiralPoints; i++)
{
    double angle = 0.5 * i;
    double radius = i * radiusIncrement;
    double x = centerX + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    FreeNode point = new FreeNode(document, x, y);
    calculatedSpline.Points.Add(point);
}

calculatedSpline.Color = 16776960; // Желтый цвет
```

## Связанные объекты
- SymmetryConstruction - Симметричный сплайн построения
- CopyConstruction - Копия сплайна построения
- OffsetConstruction - Смещенный сплайн построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества сплайнов
2. Убедитесь, что сплайны имеют достаточное количество точек для гладкости
3. Проверяйте геометрические свойства сплайнов перед использованием в сложных расчетах

## Лучшие практики
1. Используйте параметризованные сплайны для создания динамических конструкций
2. При создании больших массивов сплайнов используйте оптимизацию производительности
3. Используйте сплайны повторно при создании сложных конструкций
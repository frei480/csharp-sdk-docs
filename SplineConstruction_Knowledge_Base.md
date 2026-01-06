# SplineConstruction - База знаний для RAG-системы

## Общее описание

SplineConstruction представляет собой сплайн построения в T-Flex CAD API. Это геометрический элемент для создания гладких кривых, проходящих через заданные точки.

## Основные характеристики

- Тип: Сплайн построения
- Назначение: Создание гладких кривых через заданные точки
- Использование: Создание сложных контуров, кривых форм, траекторий движения
- Связь с другими объектами: Может использоваться как параметр для создания других геометрических объектов, источник для копирования, база для симметрии

## Конструкторы

1. `SplineConstruction(Document doc)` - Создает пустой сплайн построения

## Свойства

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

## Методы

- `AddPoint(Node point)` - Добавление точки в сплайн
- `RemovePoint(Node point)` - Удаление точки из сплайна
- `ClearPoints()` - Очистка всех точек сплайна
- `GetLength()` - Получение длины сплайна
- `GetPointAtParameter(double parameter)` - Получение точки на сплайне по параметру
- `GetTangentAtParameter(double parameter)` - Получение касательной в точке сплайна по параметру
- `IsPointOnSpline(Node point, double tolerance)` - Проверка, находится ли точка на сплайне с заданной точностью

## Паттерны использования

1. Создание сложных кривых форм
2. Определение траекторий движения
3. Создание контуров сложных объектов
4. Использование в качестве базы для CopyConstruction
5. Создание вспомогательных элементов (кривые направляющие)

## Интеграция с другими объектами

- Может быть источником для CopyConstruction
- Может использоваться как база для SymmetryConstruction
- Может быть частью PathConstruction
- Может использоваться как ограничитель для других геометрических объектов
- Может быть источником для создания ConstructionNode и OutlineNode

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

### Создание параметризованной системы сплайнов

```csharp
// Создание параметризованной системы сплайнов
int splineCount = 5;
SplineConstruction[] parametricSplines = new SplineConstruction[splineCount];

for (int i = 0; i < splineCount; i++)
{
    parametricSplines[i] = new SplineConstruction(document);
    
    // Создание точек с параметризацией
    int pointCount = 10 + i * 2;
    double yOffset = i * 15;
    
    for (int j = 0; j < pointCount; j++)
    {
        double x = 20 + j * 8;
        double y = 30 + yOffset + 10 * Math.Sin(j * 0.5 + i);
        FreeNode point = new FreeNode(document, x, y);
        parametricSplines[i].Points.Add(point);
    }
    
    // Установка цвета
    int red = (int)(255 * (double)i / (splineCount - 1));
    int green = 255 - red;
    int blue = 128;
    parametricSplines[i].Color = (red << 16) | (green << 8) | blue;
    parametricSplines[i].Style = LineStyle.Dash;
}
```

### Интеграция с другими объектами

```csharp
// Создание сплайна, интегрированного с другими объектами
SplineConstruction mainSpline = new SplineConstruction(document);

// Создание точек сплайна
FreeNode[] splinePoints = new FreeNode[6];
splinePoints[0] = new FreeNode(document, 30, 50);
splinePoints[1] = new FreeNode(document, 45, 35);
splinePoints[2] = new FreeNode(document, 60, 50);
splinePoints[3] = new FreeNode(document, 75, 65);
splinePoints[4] = new FreeNode(document, 90, 50);
splinePoints[5] = new FreeNode(document, 105, 65);

for (int i = 0; i < 6; i++)
{
    mainSpline.Points.Add(splinePoints[i]);
}

mainSpline.Color = 255; // Красный цвет

// Создание точек на сплайне
int pointOnSplineCount = 4;
FreeNode[] pointsOnSpline = new FreeNode[pointOnSplineCount];
double[] parameters = { 0.2, 0.4, 0.6, 0.8 };

for (int i = 0; i < pointOnSplineCount; i++)
{
    // В реальной реализации потребуется метод получения точки на сплайне по параметру
    // pointsOnSpline[i] = mainSpline.GetPointAtParameter(parameters[i]);
    pointsOnSpline[i] = new FreeNode(document, 
        splinePoints[1].X.Value + (splinePoints[2].X.Value - splinePoints[1].X.Value) * parameters[i],
        splinePoints[1].Y.Value + (splinePoints[2].Y.Value - splinePoints[1].Y.Value) * parameters[i]);
    
    // Создание визуальных маркеров точек
    CircleConstruction marker = new CircleConstruction(document);
    marker.SetCenterAndRadius(pointsOnSpline[i], 2);
    marker.Color = 16776960; // Желтый цвет
}
```

### Оптимизация производительности

```csharp
// Создание большого количества сплайнов с оптимизацией
int splineCount = 50;
SplineConstruction[] splines = new SplineConstruction[splineCount];
FreeNode[,] splinePoints = new FreeNode[splineCount, 5];

// Предварительное создание точек
for (int i = 0; i < splineCount; i++)
{
    for (int j = 0; j < 5; j++)
    {
        double x = 20 + (i % 10) * 15 + j * 3;
        double y = 20 + (i / 10) * 15 + j * 2;
        splinePoints[i, j] = new FreeNode(document, x, y);
    }
}

// Создание сплайнов
for (int i = 0; i < splineCount; i++)
{
    splines[i] = new SplineConstruction(document);
    for (int j = 0; j < 5; j++)
    {
        splines[i].Points.Add(splinePoints[i, j]);
    }
    // Установка цвета
    splines[i].Color = (i * 20) % 256;
}
```

### Работа с динамическими сплайнами

```csharp
// Создание динамического сплайна
SplineConstruction dynamicSpline = new SplineConstruction(document);
FreeNode[] dynamicPoints = new FreeNode[5];

// Создание точек с возможностью динамического обновления
for (int i = 0; i < 5; i++)
{
    dynamicPoints[i] = new FreeNode(document, 30 + i * 20, 50);
    dynamicSpline.Points.Add(dynamicPoints[i]);
}

dynamicSpline.Color = 16711680; // Синий цвет

// В реальном приложении здесь могла бы быть логика обновления свойств сплайна
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicSpline(double time)
{
    // Обновление точек сплайна
    for (int i = 0; i < 5; i++)
    {
        dynamicPoints[i].Y.Value = 50 + 15 * Math.Sin(time * 0.5 + i * Math.PI / 4);
    }
    
    // Обновление цвета
    int red = (int)(255 * (1 + Math.Sin(time)) / 2);
    int green = (int)(255 * (1 + Math.Cos(time + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(time + 2 * Math.PI / 3)) / 2);
    dynamicSpline.Color = (red << 16) | (green << 8) | blue;
}
*/
```

## Связанные концепции

- SymmetryConstruction - Симметричный сплайн построения
- CopyConstruction - Копия сплайна построения
- OffsetConstruction - Смещенный сплайн построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества сплайнов
2. Используйте параметризованные сплайны для создания динамических конструкций
3. При создании больших массивов сплайнов используйте оптимизацию производительности
4. Убедитесь, что сплайны имеют достаточное количество точек для гладкости
5. Используйте сплайны повторно при создании сложных конструкций
6. Проверяйте геометрические свойства сплайнов перед использованием в сложных расчетах

## Математические аспекты

- Сплайны используют математические алгоритмы интерполяции для создания гладких кривых
- Длина сплайна вычисляется численными методами
- Точки на сплайне определяются параметрически
- Касательные к сплайну вычисляются через производные
- Проверка принадлежности точки сплайну осуществляется с заданной точностью

## Совместимость и ограничения

- SplineConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях (в зависимости от узлов)
- Ограничения связаны с количеством точек и диапазоном допустимых значений координат
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- SplineConstruction может быть расширен через наследование для создания специализированных типов сплайнов
- Может быть интегрирован с пользовательскими математическими функциями
- Поддерживает пользовательские свойства через механизм параметров T-Flex
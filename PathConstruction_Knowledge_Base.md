# PathConstruction - База знаний для RAG-системы

## Общее описание

PathConstruction представляет собой путь построения в T-Flex CAD API. Это геометрический элемент для создания сложных контуров, состоящих из отдельных сегментов (линий, дуг, сплайнов и других элементов).

## Основные характеристики

- Тип: Путь построения
- Назначение: Создание сложных контуров из отдельных сегментов
- Использование: Создание контуров сложных объектов, профилей, траекторий
- Связь с другими объектами: Может использоваться как параметр для создания других геометрических объектов, источник для копирования, база для симметрии

## Конструкторы

1. `PathConstruction(Document doc)` - Создает пустой путь построения

## Свойства

- `Segments` - Коллекция сегментов пути (ConstructionCollection)
- `IsClosed` - Является ли путь замкнутым (bool)
- `GeometryType` - Тип геометрии пути построения
- `SubType` - Подтип пути построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Методы

- `AddSegment(Construction segment)` - Добавление сегмента в путь
- `AddSegment(Node startNode, Node endNode)` - Добавление линейного сегмента между двумя узлами
- `RemoveSegment(Construction segment)` - Удаление сегмента из пути
- `ClearSegments()` - Очистка всех сегментов пути
- `GetLength()` - Получение длины пути
- `GetPointAtParameter(double parameter)` - Получение точки на пути по параметру
- `GetTangentAtParameter(double parameter)` - Получение касательной в точке пути по параметру
- `IsPointOnPath(Node point, double tolerance)` - Проверка, находится ли точка на пути с заданной точностью

## Паттерны использования

1. Создание сложных контуров объектов
2. Определение профилей для выдавливания
3. Создание траекторий движения
4. Использование в качестве базы для CopyConstruction
5. Создание вспомогательных элементов (контуры, профили)

## Интеграция с другими объектами

- Может быть источником для CopyConstruction
- Может использоваться как база для SymmetryConstruction
- Может быть частью других PathConstruction
- Может использоваться как ограничитель для других геометрических объектов
- Может быть источником для создания ConstructionNode и OutlineNode

## Примеры использования

### Базовое использование

```csharp
// Создание пути из линейных сегментов
PathConstruction path = new PathConstruction(document);

// Создание узлов
FreeNode node1 = new FreeNode(document, 20, 30);
FreeNode node2 = new FreeNode(document, 50, 30);
FreeNode node3 = new FreeNode(document, 50, 60);
FreeNode node4 = new FreeNode(document, 20, 60);

// Добавление сегментов
path.AddSegment(node1, node2);
path.AddSegment(node2, node3);
path.AddSegment(node3, node4);
path.AddSegment(node4, node1); // Замыкание контура

path.Color = 255; // Красный цвет
```

### Создание пути из различных типов сегментов

```csharp
// Создание пути из различных типов сегментов
PathConstruction complexPath = new PathConstruction(document);

// Создание узлов
FreeNode startNode = new FreeNode(document, 30, 50);
FreeNode lineEndNode = new FreeNode(document, 60, 50);
FreeNode arcCenter = new FreeNode(document, 60, 60);
FreeNode arcEndNode = new FreeNode(document, 50, 70);
FreeNode splineNode1 = new FreeNode(document, 50, 70);
FreeNode splineNode2 = new FreeNode(document, 40, 80);
FreeNode splineNode3 = new FreeNode(document, 30, 70);

// Добавление линейного сегмента
LineConstruction lineSegment = new LineConstruction(document);
lineSegment.SetTwoNodes(startNode, lineEndNode);
complexPath.AddSegment(lineSegment);

// Добавление дуги (в реальной реализации потребуется ArcConstruction)
// ArcConstruction arcSegment = new ArcConstruction(document);
// arcSegment.SetCenterAndTwoPoints(arcCenter, lineEndNode, arcEndNode);
// complexPath.AddSegment(arcSegment);

// Добавление сплайна
SplineConstruction splineSegment = new SplineConstruction(document);
splineSegment.Points.Add(splineNode1);
splineSegment.Points.Add(splineNode2);
splineSegment.Points.Add(splineNode3);
complexPath.AddSegment(splineSegment);

complexPath.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание сложных контуров

```csharp
// Создание сложного контура в форме звезды
PathConstruction starPath = new PathConstruction(document);

int points = 5;
double outerRadius = 30;
double innerRadius = 15;
double centerX = 50;
double centerY = 50;

FreeNode[] starNodes = new FreeNode[points * 2];

// Создание узлов звезды
for (int i = 0; i < points * 2; i++)
{
    double radius = (i % 2 == 0) ? outerRadius : innerRadius;
    double angle = 2 * Math.PI * i / (points * 2) - Math.PI / 2;
    double x = centerX + radius * Math.Cos(angle);
    double y = centerY + radius * Math.Sin(angle);
    starNodes[i] = new FreeNode(document, x, y);
}

// Добавление сегментов
for (int i = 0; i < points * 2; i++)
{
    starPath.AddSegment(starNodes[i], starNodes[(i + 1) % (points * 2)]);
}

starPath.Color = 16711680; // Синий цвет
starPath.LineWidth = 2;
```

### Создание параметризованной системы путей

```csharp
// Создание параметризованной системы путей
int pathCount = 4;
PathConstruction[] parametricPaths = new PathConstruction[pathCount];

for (int i = 0; i < pathCount; i++)
{
    parametricPaths[i] = new PathConstruction(document);
    
    // Создание узлов с параметризацией
    int nodeCount = 4 + i;
    double xOffset = i * 30;
    double yOffset = i * 20;
    
    FreeNode[] nodes = new FreeNode[nodeCount];
    for (int j = 0; j < nodeCount; j++)
    {
        double x = 20 + xOffset + j * 15;
        double y = 30 + yOffset + 10 * Math.Sin(j * 0.5 + i);
        nodes[j] = new FreeNode(document, x, y);
    }
    
    // Добавление сегментов
    for (int j = 0; j < nodeCount - 1; j++)
    {
        parametricPaths[i].AddSegment(nodes[j], nodes[j + 1]);
    }
    
    // Замыкание контура для некоторых путей
    if (i % 2 == 0)
    {
        parametricPaths[i].AddSegment(nodes[nodeCount - 1], nodes[0]);
        parametricPaths[i].IsClosed = true;
    }
    
    // Установка цвета
    int red = (int)(255 * (double)i / (pathCount - 1));
    int green = 255 - red;
    int blue = 128;
    parametricPaths[i].Color = (red << 16) | (green << 8) | blue;
    parametricPaths[i].Style = LineStyle.Dash;
}
```

### Интеграция с другими объектами

```csharp
// Создание пути, интегрированного с другими объектами
PathConstruction mainPath = new PathConstruction(document);

// Создание узлов контура
FreeNode[] pathNodes = new FreeNode[5];
pathNodes[0] = new FreeNode(document, 30, 50);
pathNodes[1] = new FreeNode(document, 50, 30);
pathNodes[2] = new FreeNode(document, 70, 50);
pathNodes[3] = new FreeNode(document, 50, 70);
pathNodes[4] = new FreeNode(document, 30, 50); // Замыкание контура

// Добавление сегментов
for (int i = 0; i < 4; i++)
{
    mainPath.AddSegment(pathNodes[i], pathNodes[i + 1]);
}

mainPath.Color = 255; // Красный цвет

// Создание точек на пути
int pointOnPathCount = 4;
FreeNode[] pointsOnPath = new FreeNode[pointOnPathCount];
double[] parameters = { 0.2, 0.4, 0.6, 0.8 };

for (int i = 0; i < pointOnPathCount; i++)
{
    // В реальной реализации потребуется метод получения точки на пути по параметру
    // pointsOnPath[i] = mainPath.GetPointAtParameter(parameters[i]);
    // Для примера создаем точки вдоль первого сегмента
    double t = parameters[i];
    double x = pathNodes[0].X.Value + t * (pathNodes[1].X.Value - pathNodes[0].X.Value);
    double y = pathNodes[0].Y.Value + t * (pathNodes[1].Y.Value - pathNodes[0].Y.Value);
    pointsOnPath[i] = new FreeNode(document, x, y);
    
    // Создание визуальных маркеров точек
    CircleConstruction marker = new CircleConstruction(document);
    marker.SetCenterAndRadius(pointsOnPath[i], 2);
    marker.Color = 16776960; // Желтый цвет
}
```

### Оптимизация производительности

```csharp
// Создание большого количества путей с оптимизацией
int pathCount = 30;
PathConstruction[] paths = new PathConstruction[pathCount];
FreeNode[,] pathNodes = new FreeNode[pathCount, 4];

// Предварительное создание узлов
for (int i = 0; i < pathCount; i++)
{
    for (int j = 0; j < 4; j++)
    {
        double x = 20 + (i % 6) * 20 + j * 5;
        double y = 20 + (i / 6) * 20 + j * 5;
        pathNodes[i, j] = new FreeNode(document, x, y);
    }
}

// Создание путей
for (int i = 0; i < pathCount; i++)
{
    paths[i] = new PathConstruction(document);
    for (int j = 0; j < 3; j++)
    {
        paths[i].AddSegment(pathNodes[i, j], pathNodes[i, j + 1]);
    }
    // Установка цвета
    paths[i].Color = (i * 30) % 256;
}
```

### Работа с динамическими путями

```csharp
// Создание динамического пути
PathConstruction dynamicPath = new PathConstruction(document);
FreeNode[] dynamicNodes = new FreeNode[4];

// Создание узлов с возможностью динамического обновления
for (int i = 0; i < 4; i++)
{
    dynamicNodes[i] = new FreeNode(document, 30 + i * 20, 50);
    if (i > 0)
    {
        dynamicPath.AddSegment(dynamicNodes[i - 1], dynamicNodes[i]);
    }
}

dynamicPath.Color = 16711680; // Синий цвет

// В реальном приложении здесь могла бы быть логика обновления свойств пути
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicPath(double time)
{
    // Обновление узлов пути
    for (int i = 0; i < 4; i++)
    {
        dynamicNodes[i].Y.Value = 50 + 15 * Math.Sin(time * 0.5 + i * Math.PI / 4);
    }
    
    // Очистка и повторное добавление сегментов
    dynamicPath.ClearSegments();
    for (int i = 0; i < 3; i++)
    {
        dynamicPath.AddSegment(dynamicNodes[i], dynamicNodes[i + 1]);
    }
    
    // Обновление цвета
    int red = (int)(255 * (1 + Math.Sin(time)) / 2);
    int green = (int)(255 * (1 + Math.Cos(time + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(time + 2 * Math.PI / 3)) / 2);
    dynamicPath.Color = (red << 16) | (green << 8) | blue;
}
*/
```

## Связанные концепции

- SymmetryConstruction - Симметричный путь построения
- CopyConstruction - Копия пути построения
- OffsetConstruction - Смещенный путь построения
- FreeNode - Узел с абсолютными координатами
- LineConstruction - Линия построения
- SplineConstruction - Сплайн построения
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества путей
2. Используйте параметризованные пути для создания динамических конструкций
3. При создании больших массивов путей используйте оптимизацию производительности
4. Убедитесь, что пути имеют правильную топологию (корректное соединение сегментов)
5. Используйте пути повторно при создании сложных конструкций
6. Проверяйте геометрические свойства путей перед использованием в сложных расчетах

## Математические аспекты

- Длина пути вычисляется как сумма длин всех сегментов
- Точки на пути определяются параметрически по длине
- Касательные к пути вычисляются через производные отдельных сегментов
- Проверка принадлежности точки пути осуществляется с заданной точностью

## Совместимость и ограничения

- PathConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях (в зависимости от сегментов)
- Ограничения связаны с количеством сегментов и диапазоном допустимых значений координат узлов
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- PathConstruction может быть расширен через наследование для создания специализированных типов путей
- Может быть интегрирован с пользовательскими математическими функциями
- Поддерживает пользовательские свойства через механизм параметров T-Flex
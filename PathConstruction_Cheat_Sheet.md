# PathConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
PathConstruction представляет собой путь построения в T-Flex CAD API. Это геометрический элемент для создания сложных контуров, состоящих из отдельных сегментов (линий, дуг, сплайнов и других элементов).

## Основные свойства
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

## Конструкторы
```csharp
// Создание пустого пути построения
PathConstruction path = new PathConstruction(document);
```

## Основные методы
- `AddSegment(Construction segment)` - Добавление сегмента в путь
- `AddSegment(Node startNode, Node endNode)` - Добавление линейного сегмента между двумя узлами
- `RemoveSegment(Construction segment)` - Удаление сегмента из пути
- `ClearSegments()` - Очистка всех сегментов пути
- `GetLength()` - Получение длины пути
- `GetPointAtParameter(double parameter)` - Получение точки на пути по параметру
- `GetTangentAtParameter(double parameter)` - Получение касательной в точке пути по параметру
- `IsPointOnPath(Node point, double tolerance)` - Проверка, находится ли точка на пути с заданной точностью

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

## Связанные объекты
- SymmetryConstruction - Симметричный путь построения
- CopyConstruction - Копия пути построения
- OffsetConstruction - Смещенный путь построения
- FreeNode - Узел с абсолютными координатами
- LineConstruction - Линия построения
- SplineConstruction - Сплайн построения
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества путей
2. Убедитесь, что пути имеют правильную топологию (корректное соединение сегментов)
3. Проверяйте геометрические свойства путей перед использованием в сложных расчетах

## Лучшие практики
1. Используйте параметризованные пути для создания динамических конструкций
2. При создании больших массивов путей используйте оптимизацию производительности
3. Используйте пути повторно при создании сложных конструкций
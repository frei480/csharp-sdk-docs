# FreeNode - Шпаргалка по классу в T-Flex CAD API

## Описание
FreeNode представляет собой узел с абсолютными координатами в T-Flex CAD API. Это базовый элемент для создания геометрических конструкций, который определяет точку в пространстве с фиксированными координатами X и Y.

## Основные свойства
- `X` - Координата X узла (DoubleParameter)
- `Y` - Координата Y узла (DoubleParameter)
- `Z` - Координата Z узла (DoubleParameter, для 3D построений)
- `GeometryType` - Тип геометрии узла
- `SubType` - Подтип узла
- `Color` - Цвет узла
- `Layer` - Слой, на котором размещается узел
- `Level` - Уровень узла
- `Visible` - Является ли узел видимым
- `LineWidth` - Толщина линии узла
- `Style` - Стиль линии узла

## Конструкторы
```csharp
// Создание узла с координатами
FreeNode node = new FreeNode(document, x, y);
FreeNode node3D = new FreeNode(document, x, y, z);
```

## Основные методы
- `SetPosition(double x, double y)` - Установка новых координат узла
- `SetPosition(double x, double y, double z)` - Установка новых координат трехмерного узла
- `GetPosition()` - Получение текущих координат узла
- `Move(double deltaX, double deltaY)` - Перемещение узла на заданное расстояние
- `Move(double deltaX, double deltaY, double deltaZ)` - Перемещение трехмерного узла на заданное расстояние

## Примеры использования

### Базовое создание узла
```csharp
// Создание узла с координатами (50, 30)
FreeNode node = new FreeNode(document, 50, 30);
```

### Создание массива узлов
```csharp
// Создание массива узлов для многоугольника
FreeNode[] nodes = new FreeNode[6];
for (int i = 0; i < 6; i++)
{
    double angle = 2 * Math.PI * i / 6;
    nodes[i] = new FreeNode(document, 50 + 20 * Math.Cos(angle), 50 + 20 * Math.Sin(angle));
}
```

### Интеграция с другими объектами
```csharp
// Создание линии между двумя узлами
FreeNode startNode = new FreeNode(document, 20, 30);
FreeNode endNode = new FreeNode(document, 80, 30);
LineConstruction line = new LineConstruction(document);
line.SetTwoNodes(startNode, endNode);
```

## Продвинутое использование

### Параметризованные узлы
```csharp
// Создание узлов с параметризованными координатами
double centerX = 50;
double centerY = 50;
double radius = 20;
int segments = 8;
FreeNode[] nodes = new FreeNode[segments];
for (int i = 0; i < segments; i++)
{
    double angle = 2 * Math.PI * i / segments;
    nodes[i] = new FreeNode(document, centerX + radius * Math.Cos(angle), centerY + radius * Math.Sin(angle));
}
```

### Узлы с динамическими свойствами
```csharp
// Создание узлов с возможностью динамического обновления
FreeNode dynamicNode = new FreeNode(document, 50, 50);
// Позже можно изменить координаты
dynamicNode.X.Value = 60;
dynamicNode.Y.Value = 70;
```

## Связанные объекты
- LineConstruction - Линия построения
- CircleConstruction - Окружность построения
- EllipseConstruction - Эллипс построения
- SplineConstruction - Сплайн построения
- PathConstruction - Путь построения
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества узлов
2. Убедитесь, что координаты узлов находятся в допустимом диапазоне
3. Используйте узлы повторно при создании сложных конструкций

## Лучшие практики
1. Используйте параметризованные узлы для создания динамических конструкций
2. При создании больших массивов узлов используйте оптимизацию производительности
3. Проверяйте геометрические свойства узлов перед использованием в сложных расчетах
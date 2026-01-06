# LineConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
LineConstruction представляет собой линию построения в T-Flex CAD API. Это базовый элемент для создания геометрических конструкций, который определяет прямую линию между двумя точками.

## Основные свойства
- `Node1` - Первый узел линии (Node)
- `Node2` - Второй узел линии (Node)
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
// Создание пустой линии построения
LineConstruction line = new LineConstruction(document);
// Создание линии между двумя узлами
LineConstruction line = new LineConstruction(document, node1, node2);
```

## Основные методы
- `SetTwoNodes(Node node1, Node node2)` - Установка двух узлов линии
- `GetLength()` - Получение длины линии
- `GetAngle()` - Получение угла наклона линии
- `GetMidPoint()` - Получение средней точки линии
- `IsParallelTo(LineConstruction other)` - Проверка параллельности с другой линией
- `IsPerpendicularTo(LineConstruction other)` - Проверка перпендикулярности с другой линией
- `GetIntersectionWith(LineConstruction other)` - Получение точки пересечения с другой линией

## Примеры использования

### Базовое использование
```csharp
// Создание линии между двумя узлами
FreeNode startNode = new FreeNode(document, 20, 30);
FreeNode endNode = new FreeNode(document, 80, 30);
LineConstruction line = new LineConstruction(document);
line.SetTwoNodes(startNode, endNode);
```

### Создание линии с определенными свойствами
```csharp
// Создание линии с заданными свойствами
FreeNode node1 = new FreeNode(document, 30, 40);
FreeNode node2 = new FreeNode(document, 70, 80);
LineConstruction line = new LineConstruction(document);
line.SetTwoNodes(node1, node2);
line.Color = 255; // Красный цвет
line.LineWidth = 2;
line.Style = LineStyle.Solid;
```

### Интеграция с симметрией
```csharp
// Создание линии как оси симметрии
FreeNode axisStart = new FreeNode(document, 50, 20);
FreeNode axisEnd = new FreeNode(document, 50, 80);
LineConstruction symmetryAxis = new LineConstruction(document);
symmetryAxis.SetTwoNodes(axisStart, axisEnd);

// Использование линии как оси симметрии
SymmetryConstruction symmetry = new SymmetryConstruction(document);
// symmetry.Source = sourceObject;
symmetry.Axis = symmetryAxis;
```

## Продвинутое использование

### Создание параметризованных линий
```csharp
// Создание линии с параметризованными координатами
double startX = 30;
double startY = 40;
double length = 50;
double angle = Math.PI / 4; // 45 градусов
FreeNode startNode = new FreeNode(document, startX, startY);
FreeNode endNode = new FreeNode(document, 
    startX + length * Math.Cos(angle), 
    startY + length * Math.Sin(angle));
LineConstruction parametricLine = new LineConstruction(document);
parametricLine.SetTwoNodes(startNode, endNode);
```

### Создание линий с геометрическими расчетами
```csharp
// Создание перпендикулярной линии
LineConstruction originalLine = new LineConstruction(document);
originalLine.SetTwoNodes(new FreeNode(document, 20, 30), new FreeNode(document, 80, 30));

// Создание перпендикулярной линии через среднюю точку
double midX = (originalLine.Node1.X.Value + originalLine.Node2.X.Value) / 2;
double midY = (originalLine.Node1.Y.Value + originalLine.Node2.Y.Value) / 2;
FreeNode midPoint = new FreeNode(document, midX, midY);

// Создание перпендикулярной линии длиной 30
double originalAngle = Math.Atan2(
    originalLine.Node2.Y.Value - originalLine.Node1.Y.Value,
    originalLine.Node2.X.Value - originalLine.Node1.X.Value);
double perpendicularAngle = originalAngle + Math.PI / 2;
double length = 30;
FreeNode endPoint = new FreeNode(document, 
    midX + length * Math.Cos(perpendicularAngle), 
    midY + length * Math.Sin(perpendicularAngle));

LineConstruction perpendicularLine = new LineConstruction(document);
perpendicularLine.SetTwoNodes(midPoint, endPoint);
```

## Связанные объекты
- SymmetryConstruction - Симметричная линия построения
- CopyConstruction - Копия линии построения
- OffsetConstruction - Смещенная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества линий
2. Убедитесь, что узлы линий находятся в допустимом диапазоне
3. Проверяйте геометрические свойства линий перед использованием в сложных расчетах

## Лучшие практики
1. Используйте параметризованные линии для создания динамических конструкций
2. При создании больших массивов линий используйте оптимизацию производительности
3. Используйте линии повторно при создании сложных конструкций
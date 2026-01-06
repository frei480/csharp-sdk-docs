# LineConstruction - База знаний для RAG-системы

## Общее описание

LineConstruction представляет собой линию построения в T-Flex CAD API. Это базовый элемент для создания геометрических конструкций, который определяет прямую линию между двумя точками.

## Основные характеристики

- Тип: Линия построения
- Назначение: Создание прямых линий между двумя точками
- Использование: Основа для более сложных геометрических конструкций, оси симметрии, направляющие линии
- Связь с другими объектами: Может использоваться как параметр для создания других геометрических объектов, ось для симметрии, источник для копирования

## Конструкторы

1. `LineConstruction(Document doc)` - Создает пустую линию построения
2. `LineConstruction(Document doc, Node node1, Node node2)` - Создает линию между двумя узлами

## Свойства

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

## Методы

- `SetTwoNodes(Node node1, Node node2)` - Установка двух узлов линии
- `GetLength()` - Получение длины линии
- `GetAngle()` - Получение угла наклона линии
- `GetMidPoint()` - Получение средней точки линии
- `IsParallelTo(LineConstruction other)` - Проверка параллельности с другой линией
- `IsPerpendicularTo(LineConstruction other)` - Проверка перпендикулярности с другой линией
- `GetIntersectionWith(LineConstruction other)` - Получение точки пересечения с другой линией

## Паттерны использования

1. Создание осей симметрии для SymmetryConstruction
2. Определение направляющих линий для других конструкций
3. Создание ограничительных линий для геометрических объектов
4. Использование в качестве базы для CopyConstruction
5. Создание сеток и вспомогательных конструкций

## Интеграция с другими объектами

- Используется как ось для SymmetryConstruction
- Может быть источником для CopyConstruction
- Может использоваться для создания OffsetConstruction
- Может быть частью PathConstruction
- Может использоваться как ограничитель для других геометрических объектов

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

### Создание массива линий

```csharp
// Создание сетки из линий
int rows = 5;
int cols = 5;
double spacing = 20;
double startX = 20;
double startY = 20;

LineConstruction[,] horizontalLines = new LineConstruction[rows + 1, cols];
LineConstruction[,] verticalLines = new LineConstruction[rows, cols + 1];

// Создание горизонтальных линий
for (int i = 0; i <= rows; i++)
{
    for (int j = 0; j < cols; j++)
    {
        FreeNode start = new FreeNode(document, startX + j * spacing, startY + i * spacing);
        FreeNode end = new FreeNode(document, startX + (j + 1) * spacing, startY + i * spacing);
        horizontalLines[i, j] = new LineConstruction(document);
        horizontalLines[i, j].SetTwoNodes(start, end);
        horizontalLines[i, j].Color = 12632256; // Серый цвет
        horizontalLines[i, j].Style = LineStyle.Dash; // Пунктирная линия
    }
}

// Создание вертикальных линий
for (int i = 0; i < rows; i++)
{
    for (int j = 0; j <= cols; j++)
    {
        FreeNode start = new FreeNode(document, startX + j * spacing, startY + i * spacing);
        FreeNode end = new FreeNode(document, startX + j * spacing, startY + (i + 1) * spacing);
        verticalLines[i, j] = new LineConstruction(document);
        verticalLines[i, j].SetTwoNodes(start, end);
        verticalLines[i, j].Color = 12632256; // Серый цвет
        verticalLines[i, j].Style = LineStyle.Dash; // Пунктирная линия
    }
}
```

## Связанные концепции

- SymmetryConstruction - Симметричная линия построения
- CopyConstruction - Копия линии построения
- OffsetConstruction - Смещенная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества линий
2. Используйте параметризованные линии для создания динамических конструкций
3. При создании больших массивов линий используйте оптимизацию производительности
4. Убедитесь, что узлы линий находятся в допустимом диапазоне
5. Используйте линии повторно при создании сложных конструкций
6. Проверяйте геометрические свойства линий перед использованием в сложных расчетах

## Математические аспекты

- Длина линии вычисляется по формуле расстояния между двумя точками
- Угол наклона линии вычисляется с использованием арктангенса
- Пересечения линий вычисляются с использованием линейной алгебры
- Параллельность и перпендикулярность определяются через наклоны линий

## Совместимость и ограничения

- LineConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях (в зависимости от узлов)
- Ограничения связаны с диапазоном допустимых значений координат узлов
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- LineConstruction может быть расширен через наследование для создания специализированных типов линий
- Может быть интегрирован с пользовательскими математическими функциями
- Поддерживает пользовательские свойства через механизм параметров T-Flex
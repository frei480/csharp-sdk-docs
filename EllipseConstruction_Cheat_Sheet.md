# EllipseConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
EllipseConstruction представляет собой эллипс построения в T-Flex CAD API. Это геометрический элемент для создания эллипсов с заданными параметрами центра и полуосей.

## Основные свойства
- `Center` - Центр эллипса (Node)
- `MajorNode` - Узел большой полуоси (Node)
- `MinorNode` - Узел малой полуоси (Node)
- `MajorRadius` - Большая полуось (DoubleParameter)
- `MinorRadius` - Малая полуось (DoubleParameter)
- `GeometryType` - Тип геометрии эллипса построения
- `SubType` - Подтип эллипса построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Конструкторы
```csharp
// Создание пустого эллипса построения
EllipseConstruction ellipse = new EllipseConstruction(document);
// Создание эллипса с заданным центром и узлами полуосей
EllipseConstruction ellipse = new EllipseConstruction(document, center, majorNode, minorNode);
```

## Основные методы
- `SetCenterAndTwoNodes(Node center, Node majorNode, Node minorNode)` - Установка центра и узлов полуосей
- `SetCenterAndRadii(Node center, double majorRadius, double minorRadius)` - Установка центра и радиусов полуосей
- `GetArea()` - Получение площади эллипса
- `GetPerimeter()` - Получение периметра эллипса (приближенное значение)
- `IsPointInside(Node point)` - Проверка, находится ли точка внутри эллипса
- `GetTangentLine(Node point)` - Получение касательной линии в заданной точке
- `GetIntersectionWith(LineConstruction line)` - Получение точек пересечения с линией

## Примеры использования

### Базовое использование
```csharp
// Создание эллипса с заданным центром и узлами полуосей
FreeNode center = new FreeNode(document, 50, 50);
FreeNode majorNode = new FreeNode(document, 70, 50); // Большая полуось по X
FreeNode minorNode = new FreeNode(document, 50, 60); // Малая полуось по Y
EllipseConstruction ellipse = new EllipseConstruction(document);
ellipse.SetCenterAndTwoNodes(center, majorNode, minorNode);
```

### Создание эллипса с радиусами
```csharp
// Создание эллипса с заданными радиусами полуосей
FreeNode center = new FreeNode(document, 50, 50);
EllipseConstruction ellipse = new EllipseConstruction(document);
ellipse.SetCenterAndRadii(center, 20, 10); // Большая полуось 20, малая 10
```

### Создание эллипса с определенными свойствами
```csharp
// Создание эллипса с заданными свойствами
FreeNode center = new FreeNode(document, 50, 50);
FreeNode majorNode = new FreeNode(document, 75, 50);
FreeNode minorNode = new FreeNode(document, 50, 65);
EllipseConstruction ellipse = new EllipseConstruction(document);
ellipse.SetCenterAndTwoNodes(center, majorNode, minorNode);
ellipse.Color = 255; // Красный цвет
ellipse.LineWidth = 2;
ellipse.Style = LineStyle.Solid;
```

## Продвинутое использование

### Создание концентрических эллипсов
```csharp
// Создание набора концентрических эллипсов
FreeNode center = new FreeNode(document, 50, 50);
int count = 5;
double baseMajorRadius = 20;
double baseMinorRadius = 10;
double spacing = 3;

EllipseConstruction[] concentricEllipses = new EllipseConstruction[count];
for (int i = 0; i < count; i++)
{
    concentricEllipses[i] = new EllipseConstruction(document);
    concentricEllipses[i].SetCenterAndRadii(
        center, 
        baseMajorRadius + i * spacing, 
        baseMinorRadius + i * spacing / 2);
    // Установка различных цветов для каждого эллипса
    concentricEllipses[i].Color = (i * 50) << 16 | ((count - i) * 50) << 8 | 128;
    concentricEllipses[i].Style = LineStyle.Dash;
}
```

### Создание эллипсов с геометрическими расчетами
```csharp
// Создание эллипсов на основе геометрических расчетов
FreeNode[] centers = new FreeNode[4];
centers[0] = new FreeNode(document, 30, 30);
centers[1] = new FreeNode(document, 70, 30);
centers[2] = new FreeNode(document, 70, 70);
centers[3] = new FreeNode(document, 30, 70);

EllipseConstruction[] calculatedEllipses = new EllipseConstruction[4];
for (int i = 0; i < 4; i++)
{
    calculatedEllipses[i] = new EllipseConstruction(document);
    // Радиусы рассчитываются как расстояния до центра координат
    double majorRadius = Math.Sqrt(
        Math.Pow(centers[i].X.Value, 2) + 
        Math.Pow(centers[i].Y.Value, 2)) / 15;
    double minorRadius = majorRadius * 0.7;
    calculatedEllipses[i].SetCenterAndRadii(centers[i], majorRadius, minorRadius);
    calculatedEllipses[i].Color = 65280; // Зеленый цвет
}
```

## Связанные объекты
- SymmetryConstruction - Симметричный эллипс построения
- CopyConstruction - Копия эллипса построения
- OffsetConstruction - Смещенный эллипс построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества эллипсов
2. Убедитесь, что радиусы полуосей положительные
3. Проверяйте геометрические свойства эллипсов перед использованием в сложных расчетах

## Лучшие практики
1. Используйте параметризованные эллипсы для создания динамических конструкций
2. При создании больших массивов эллипсов используйте оптимизацию производительности
3. Используйте эллипсы повторно при создании сложных конструкций
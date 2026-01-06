# CircleConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
CircleConstruction представляет собой окружность построения в T-Flex CAD API. Это геометрический элемент для создания окружностей с заданными параметрами центра и радиуса.

## Основные свойства
- `Center` - Центр окружности (Node)
- `Radius` - Радиус окружности (DoubleParameter)
- `GeometryType` - Тип геометрии окружности построения
- `SubType` - Подтип окружности построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Конструкторы
```csharp
// Создание пустой окружности построения
CircleConstruction circle = new CircleConstruction(document);
// Создание окружности с заданным центром и радиусом
CircleConstruction circle = new CircleConstruction(document, center, radius);
```

## Основные методы
- `SetCenterAndRadius(Node center, double radius)` - Установка центра и радиуса окружности
- `SetCenterAndPoint(Node center, Node point)` - Установка центра и точки на окружности
- `GetArea()` - Получение площади окружности
- `GetCircumference()` - Получение длины окружности
- `IsPointInside(Node point)` - Проверка, находится ли точка внутри окружности
- `GetTangentLine(Node point)` - Получение касательной линии в заданной точке
- `GetIntersectionWith(LineConstruction line)` - Получение точек пересечения с линией

## Примеры использования

### Базовое использование
```csharp
// Создание окружности с заданным центром и радиусом
FreeNode center = new FreeNode(document, 50, 50);
CircleConstruction circle = new CircleConstruction(document);
circle.SetCenterAndRadius(center, 20);
```

### Создание окружности через центр и точку
```csharp
// Создание окружности через центр и точку на окружности
FreeNode center = new FreeNode(document, 50, 50);
FreeNode point = new FreeNode(document, 70, 50);
CircleConstruction circle = new CircleConstruction(document);
circle.SetCenterAndPoint(center, point);
```

### Создание окружности с определенными свойствами
```csharp
// Создание окружности с заданными свойствами
FreeNode center = new FreeNode(document, 50, 50);
CircleConstruction circle = new CircleConstruction(document);
circle.SetCenterAndRadius(center, 15);
circle.Color = 255; // Красный цвет
circle.LineWidth = 2;
circle.Style = LineStyle.Solid;
```

## Продвинутое использование

### Создание концентрических окружностей
```csharp
// Создание набора концентрических окружностей
FreeNode center = new FreeNode(document, 50, 50);
int count = 5;
double baseRadius = 10;
double spacing = 5;

CircleConstruction[] concentricCircles = new CircleConstruction[count];
for (int i = 0; i < count; i++)
{
    concentricCircles[i] = new CircleConstruction(document);
    concentricCircles[i].SetCenterAndRadius(center, baseRadius + i * spacing);
    // Установка различных цветов для каждой окружности
    concentricCircles[i].Color = (i * 50) << 16 | ((count - i) * 50) << 8 | 128;
    concentricCircles[i].Style = LineStyle.Dash;
}
```

### Создание окружностей с геометрическими расчетами
```csharp
// Создание окружностей на основе геометрических расчетов
FreeNode[] centers = new FreeNode[4];
centers[0] = new FreeNode(document, 30, 30);
centers[1] = new FreeNode(document, 70, 30);
centers[2] = new FreeNode(document, 70, 70);
centers[3] = new FreeNode(document, 30, 70);

CircleConstruction[] calculatedCircles = new CircleConstruction[4];
for (int i = 0; i < 4; i++)
{
    calculatedCircles[i] = new CircleConstruction(document);
    // Радиус рассчитывается как расстояние до центра координат
    double radius = Math.Sqrt(
        Math.Pow(centers[i].X.Value, 2) + 
        Math.Pow(centers[i].Y.Value, 2)) / 10;
    calculatedCircles[i].SetCenterAndRadius(centers[i], radius);
    calculatedCircles[i].Color = 65280; // Зеленый цвет
}
```

## Связанные объекты
- SymmetryConstruction - Симметричная окружность построения
- CopyConstruction - Копия окружности построения
- OffsetConstruction - Смещенная окружность построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества окружностей
2. Убедитесь, что радиус окружности положительный
3. Проверяйте геометрические свойства окружностей перед использованием в сложных расчетах

## Лучшие практики
1. Используйте параметризованные окружности для создания динамических конструкций
2. При создании больших массивов окружностей используйте оптимизацию производительности
3. Используйте окружности повторно при создании сложных конструкций
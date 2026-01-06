# CircleConstruction - База знаний для RAG-системы

## Общее описание

CircleConstruction представляет собой окружность построения в T-Flex CAD API. Это геометрический элемент для создания окружностей с заданными параметрами центра и радиуса.

## Основные характеристики

- Тип: Окружность построения
- Назначение: Создание окружностей с заданными параметрами
- Использование: Основа для более сложных геометрических конструкций, создание отверстий, контуров, вспомогательных элементов
- Связь с другими объектами: Может использоваться как параметр для создания других геометрических объектов, источник для копирования, база для симметрии

## Конструкторы

1. `CircleConstruction(Document doc)` - Создает пустую окружность построения
2. `CircleConstruction(Document doc, Node center, double radius)` - Создает окружность с заданным центром и радиусом

## Свойства

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

## Методы

- `SetCenterAndRadius(Node center, double radius)` - Установка центра и радиуса окружности
- `SetCenterAndPoint(Node center, Node point)` - Установка центра и точки на окружности
- `GetArea()` - Получение площади окружности
- `GetCircumference()` - Получение длины окружности
- `IsPointInside(Node point)` - Проверка, находится ли точка внутри окружности
- `GetTangentLine(Node point)` - Получение касательной линии в заданной точке
- `GetIntersectionWith(LineConstruction line)` - Получение точек пересечения с линией

## Паттерны использования

1. Создание базовых окружностей для других конструкций
2. Определение отверстий и контуров
3. Создание концентрических окружностей
4. Использование в качестве базы для CopyConstruction
5. Создание вспомогательных элементов (оси, центры)

## Интеграция с другими объектами

- Может быть источником для CopyConstruction
- Может использоваться как база для SymmetryConstruction
- Может быть частью PathConstruction
- Может использоваться как ограничитель для других геометрических объектов
- Может быть источником для создания ConstructionNode и OutlineNode

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

### Создание параметризованной системы окружностей

```csharp
// Создание параметризованной системы окружностей
double centerX = 50;
double centerY = 50;
int paramCount = 8;
double baseRadius = 15;
double radiusIncrement = 3;

CircleConstruction[] parametricCircles = new CircleConstruction[paramCount];
for (int i = 0; i < paramCount; i++)
{
    double angle = 2 * Math.PI * i / paramCount;
    double x = centerX + (baseRadius + i * radiusIncrement) * Math.Cos(angle);
    double y = centerY + (baseRadius + i * radiusIncrement) * Math.Sin(angle);
    
    FreeNode center = new FreeNode(document, x, y);
    parametricCircles[i] = new CircleConstruction(document);
    parametricCircles[i].SetCenterAndRadius(center, baseRadius + i * radiusIncrement / 2);
    
    // Установка цвета в зависимости от параметра
    int red = (int)(255 * (double)i / (paramCount - 1));
    int green = 255 - red;
    int blue = 128;
    parametricCircles[i].Color = (red << 16) | (green << 8) | blue;
}
```

### Интеграция с другими объектами

```csharp
// Создание окружностей, интегрированных с линиями
FreeNode center = new FreeNode(document, 50, 50);
CircleConstruction mainCircle = new CircleConstruction(document);
mainCircle.SetCenterAndRadius(center, 25);
mainCircle.Color = 255; // Красный цвет

// Создание радиальных линий
int lineCount = 8;
LineConstruction[] radialLines = new LineConstruction[lineCount];
for (int i = 0; i < lineCount; i++)
{
    double angle = 2 * Math.PI * i / lineCount;
    double x = center.X.Value + 25 * Math.Cos(angle);
    double y = center.Y.Value + 25 * Math.Sin(angle);
    
    FreeNode endPoint = new FreeNode(document, x, y);
    radialLines[i] = new LineConstruction(document);
    radialLines[i].SetTwoNodes(center, endPoint);
    radialLines[i].Color = 12632256; // Серый цвет
    radialLines[i].Style = LineStyle.Dash;
}
```

### Оптимизация производительности

```csharp
// Создание большого количества окружностей с оптимизацией
int circleCount = 100;
CircleConstruction[] circles = new CircleConstruction[circleCount];
FreeNode[] centers = new FreeNode[circleCount];

// Предварительное создание центров
for (int i = 0; i < circleCount; i++)
{
    double x = 20 + (i % 10) * 15;
    double y = 20 + (i / 10) * 15;
    centers[i] = new FreeNode(document, x, y);
}

// Создание окружностей
for (int i = 0; i < circleCount; i++)
{
    circles[i] = new CircleConstruction(document);
    circles[i].SetCenterAndRadius(centers[i], 3 + (i % 3));
    // Установка цвета
    circles[i].Color = (i * 10) % 256;
}
```

### Работа с динамическими окружностями

```csharp
// Создание динамической окружности
FreeNode dynamicCenter = new FreeNode(document, 50, 50);
CircleConstruction dynamicCircle = new CircleConstruction(document);
dynamicCircle.SetCenterAndRadius(dynamicCenter, 15);
dynamicCircle.Color = 16711680; // Синий цвет

// В реальном приложении здесь могла бы быть логика обновления свойств окружности
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicCircle(double time)
{
    // Обновление центра
    dynamicCenter.X.Value = 50 + 20 * Math.Sin(time * 0.5);
    dynamicCenter.Y.Value = 50 + 20 * Math.Cos(time * 0.5);
    
    // Обновление радиуса
    dynamicCircle.Radius.Value = 15 + 5 * Math.Sin(time * 2);
    
    // Обновление цвета
    int red = (int)(255 * (1 + Math.Sin(time)) / 2);
    int green = (int)(255 * (1 + Math.Cos(time + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(time + 2 * Math.PI / 3)) / 2);
    dynamicCircle.Color = (red << 16) | (green << 8) | blue;
}
*/
```

## Связанные концепции

- SymmetryConstruction - Симметричная окружность построения
- CopyConstruction - Копия окружности построения
- OffsetConstruction - Смещенная окружность построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества окружностей
2. Используйте параметризованные окружности для создания динамических конструкций
3. При создании больших массивов окружностей используйте оптимизацию производительности
4. Убедитесь, что радиус окружности положительный
5. Используйте окружности повторно при создании сложных конструкций
6. Проверяйте геометрические свойства окружностей перед использованием в сложных расчетах

## Математические аспекты

- Площадь окружности вычисляется по формуле π*r²
- Длина окружности вычисляется по формуле 2*π*r
- Проверка принадлежности точки окружности осуществляется через расстояние до центра
- Касательные линии вычисляются с использованием геометрических формул
- Пересечения с линиями вычисляются с использованием алгебраических методов

## Совместимость и ограничения

- CircleConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях (в зависимости от узлов)
- Ограничения связаны с диапазоном допустимых значений радиуса и координат центра
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- CircleConstruction может быть расширен через наследование для создания специализированных типов окружностей
- Может быть интегрирован с пользовательскими математическими функциями
- Поддерживает пользовательские свойства через механизм параметров T-Flex
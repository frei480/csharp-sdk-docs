# OffsetConstruction - База знаний для RAG-системы

## Общее описание

OffsetConstruction представляет собой смещенную линию построения в T-Flex CAD API. Это геометрический элемент для создания параллельных копий других геометрических объектов на заданном расстоянии.

## Основные характеристики

- Тип: Смещенная линия построения
- Назначение: Создание параллельных копий геометрических объектов
- Использование: Создание контуров, траекторий, параллельных линий
- Связь с другими объектами: Использует другие геометрические объекты как источник, создает параллельные копии

## Конструкторы

1. `OffsetConstruction(Document doc)` - Создает пустую смещенную линию построения

## Свойства

- `Source` - Исходная линия построения (Construction)
- `Distance` - Расстояние смещения (DoubleParameter)
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Методы

- `SetSource(Construction source)` - Установка исходного объекта
- `SetDistance(double distance)` - Установка расстояния смещения
- `GetOffsetGeometry()` - Получение смещенной геометрии
- `GetNormalVectorAtPoint(Node point)` - Получение вектора нормали в точке

## Паттерны использования

1. Создание параллельных линий
2. Создание контуров объектов
3. Генерация траекторий движения
4. Создание границ зон безопасности
5. Построение эквидистантных кривых

## Интеграция с другими объектами

- Использует любые Construction объекты как источник
- Может быть источником для других OffsetConstruction
- Может использоваться как база для CopyConstruction
- Может быть частью PathConstruction
- Может использоваться как ограничитель для других геометрических объектов

## Примеры использования

### Базовое использование

```csharp
// Создание простого смещения линии
LineConstruction originalLine = new LineConstruction(document);
originalLine.SetTwoNodes(new FreeNode(document, 30, 50), new FreeNode(document, 70, 50));

OffsetConstruction offset = new OffsetConstruction(document);
offset.SetSource(originalLine);
offset.SetDistance(10); // Смещение на 10 единиц вверх
offset.Color = 255; // Красный цвет
```

### Создание смещения контура

```csharp
// Создание смещения замкнутого контура
PathConstruction originalPath = new PathConstruction(document);

// Создание прямоугольного контура
FreeNode[] nodes = new FreeNode[4];
nodes[0] = new FreeNode(document, 40, 40);
nodes[1] = new FreeNode(document, 60, 40);
nodes[2] = new FreeNode(document, 60, 60);
nodes[3] = new FreeNode(document, 40, 60);

for (int i = 0; i < 4; i++)
{
    originalPath.AddSegment(nodes[i], nodes[(i + 1) % 4]);
}

OffsetConstruction pathOffset = new OffsetConstruction(document);
pathOffset.SetSource(originalPath);
pathOffset.SetDistance(5); // Смещение на 5 единиц внутрь
pathOffset.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание множественных смещений

```csharp
// Создание множественных смещений
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 50, 50), 20);

int offsetCount = 5;
double baseDistance = 5;
OffsetConstruction[] offsets = new OffsetConstruction[offsetCount];

for (int i = 0; i < offsetCount; i++)
{
    offsets[i] = new OffsetConstruction(document);
    offsets[i].SetSource(originalCircle);
    offsets[i].SetDistance(baseDistance * (i + 1));
    
    // Установка цвета с градиентом
    int red = (int)(255 * (double)i / (offsetCount - 1));
    int green = 255 - red;
    int blue = 128;
    offsets[i].Color = (red << 16) | (green << 8) | blue;
    offsets[i].Style = LineStyle.Dash;
}
```

### Создание смещений с геометрическими расчетами

```csharp
// Создание смещений с геометрическими расчетами
SplineConstruction originalSpline = new SplineConstruction(document);

// Создание точек сплайна в форме волны
int pointCount = 10;
for (int i = 0; i < pointCount; i++)
{
    double x = 20 + i * 8;
    double y = 50 + 15 * Math.Sin(i * 0.5);
    FreeNode point = new FreeNode(document, x, y);
    originalSpline.Points.Add(point);
}

// Создание смещений в обе стороны
OffsetConstruction[] splineOffsets = new OffsetConstruction[2];
double[] distances = { 5, -5 }; // В обе стороны от сплайна

for (int i = 0; i < 2; i++)
{
    splineOffsets[i] = new OffsetConstruction(document);
    splineOffsets[i].SetSource(originalSpline);
    splineOffsets[i].SetDistance(distances[i]);
    splineOffsets[i].Color = (i == 0) ? 255 : 16711680; // Красный и синий
    splineOffsets[i].Style = LineStyle.Dash;
}
```

### Создание параметризованной системы смещений

```csharp
// Создание параметризованной системы смещений
EllipseConstruction originalEllipse = new EllipseConstruction(document);
originalEllipse.SetCenterAndRadii(new FreeNode(document, 50, 50), 25, 15);

int parametricCount = 8;
OffsetConstruction[] parametricOffsets = new OffsetConstruction[parametricCount];

for (int i = 0; i < parametricCount; i++)
{
    parametricOffsets[i] = new OffsetConstruction(document);
    parametricOffsets[i].SetSource(originalEllipse);
    
    // Параметрическое расстояние смещения
    double distance = 3 + i * 2;
    parametricOffsets[i].SetDistance(distance);
    
    // Установка цвета
    int red = (int)(255 * (double)i / (parametricCount - 1));
    int green = 255 - red;
    int blue = 128;
    parametricOffsets[i].Color = (red << 16) | (green << 8) | blue;
    parametricOffsets[i].Style = LineStyle.Dash;
}
```

### Интеграция с другими объектами

```csharp
// Создание смещений, интегрированных с другими объектами
PathConstruction originalPath = new PathConstruction(document);

// Создание контура в форме треугольника
FreeNode[] triangleNodes = new FreeNode[3];
triangleNodes[0] = new FreeNode(document, 50, 30);
triangleNodes[1] = new FreeNode(document, 30, 70);
triangleNodes[2] = new FreeNode(document, 70, 70);

for (int i = 0; i < 3; i++)
{
    originalPath.AddSegment(triangleNodes[i], triangleNodes[(i + 1) % 3]);
}

// Создание смещения контура
OffsetConstruction pathOffset = new OffsetConstruction(document);
pathOffset.SetSource(originalPath);
pathOffset.SetDistance(8);
pathOffset.Color = 16711680; // Синий цвет

// Создание вспомогательных линий нормалей
int normalCount = 3;
LineConstruction[] normalLines = new LineConstruction[normalCount];
// В реальной реализации потребуется метод получения нормали в точке
// Для примера создаем приблизительные нормали
double[] normalAngles = { Math.PI / 2, -Math.PI / 4, -3 * Math.PI / 4 };

for (int i = 0; i < normalCount; i++)
{
    double centerX = triangleNodes[i].X.Value;
    double centerY = triangleNodes[i].Y.Value;
    
    // Создание линии нормали
    FreeNode startPoint = new FreeNode(document, centerX, centerY);
    FreeNode endPoint = new FreeNode(document, 
        centerX + 10 * Math.Cos(normalAngles[i]), 
        centerY + 10 * Math.Sin(normalAngles[i]));
    
    normalLines[i] = new LineConstruction(document);
    normalLines[i].SetTwoNodes(startPoint, endPoint);
    normalLines[i].Color = 12632256; // Серый цвет
    normalLines[i].Style = LineStyle.Dash;
}
```

### Оптимизация производительности

```csharp
// Создание большого количества смещений с оптимизацией
int offsetCount = 50;
OffsetConstruction[] offsets = new OffsetConstruction[offsetCount];
LineConstruction[] sourceLines = new LineConstruction[10];

// Создание небольшого количества исходных линий
for (int i = 0; i < 10; i++)
{
    sourceLines[i] = new LineConstruction(document);
    sourceLines[i].SetTwoNodes(
        new FreeNode(document, 20 + i * 8, 40), 
        new FreeNode(document, 20 + i * 8, 60));
}

// Создание смещений с использованием ограниченного набора источников
for (int i = 0; i < offsetCount; i++)
{
    offsets[i] = new OffsetConstruction(document);
    offsets[i].SetSource(sourceLines[i % 10]);
    offsets[i].SetDistance(2 + (i % 5)); // Различные расстояния
    // Установка цвета
    offsets[i].Color = (i * 20) % 256;
}
```

### Работа с динамическими смещениями

```csharp
// Создание динамического смещения
CircleConstruction dynamicSource = new CircleConstruction(document);
dynamicSource.SetCenterAndRadius(new FreeNode(document, 50, 50), 15);

OffsetConstruction dynamicOffset = new OffsetConstruction(document);
dynamicOffset.SetSource(dynamicSource);
dynamicOffset.SetDistance(10);
dynamicOffset.Color = 16711680; // Синий цвет

// В реальном приложении здесь могла бы быть логика обновления свойств смещения
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicOffset(double time)
{
    // Обновление расстояния смещения
    double distance = 5 + 10 * Math.Abs(Math.Sin(time * 0.5));
    dynamicOffset.SetDistance(distance);
    
    // Обновление цвета
    int red = (int)(255 * (1 + Math.Sin(time)) / 2);
    int green = (int)(255 * (1 + Math.Cos(time + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(time + 2 * Math.PI / 3)) / 2);
    dynamicOffset.Color = (red << 16) | (green << 8) | blue;
}
*/
```

## Связанные концепции

- CopyConstruction - Копия линии построения
- SymmetryConstruction - Симметричная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества смещений
2. Используйте параметризованные смещения для создания динамических конструкций
3. При создании больших массивов смещений используйте оптимизацию производительности
4. Убедитесь, что исходные объекты существуют и корректны
5. Проверяйте допустимые значения расстояний смещения
6. Используйте смещения повторно при создании сложных конструкций

## Математические аспекты

- Смещения вычисляются через нормали к исходным кривым
- Расстояние смещения измеряется по перпендикуляру к исходной кривой
- Для сложных кривых вычисления смещений могут быть приближенными
- Направление смещения определяется знаком расстояния

## Совместимость и ограничения

- OffsetConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях
- Ограничения связаны с геометрической сложностью исходных объектов
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- OffsetConstruction может быть расширен через наследование для создания специализированных типов смещений
- Может быть интегрирован с пользовательскими математическими функциями вычисления нормалей
- Поддерживает пользовательские свойства через механизм параметров T-Flex
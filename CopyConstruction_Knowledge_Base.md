# CopyConstruction - База знаний для RAG-системы

## Общее описание

CopyConstruction представляет собой копию линии построения в T-Flex CAD API. Это геометрический элемент для создания копий других геометрических объектов с применением трансформаций.

## Основные характеристики

- Тип: Копия линии построения
- Назначение: Создание копий других геометрических объектов
- Использование: Создание массивов объектов, повторяющихся элементов, применение трансформаций
- Связь с другими объектами: Использует другие геометрические объекты как источник, применяет к ним трансформации

## Конструкторы

1. `CopyConstruction(Document doc)` - Создает пустую копию линии построения

## Свойства

- `Source` - Исходная линия построения (Construction)
- `Matrix` - Матрица трансформации (Matrix3D)
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
- `SetMatrix(Matrix3D matrix)` - Установка матрицы трансформации
- `SetTranslation(double dx, double dy, double dz)` - Установка трансляции
- `SetRotation(double angle, double axisX, double axisY, double axisZ)` - Установка вращения
- `SetScale(double scaleX, double scaleY, double scaleZ)` - Установка масштабирования
- `GetTransformedGeometry()` - Получение трансформированной геометрии

## Паттерны использования

1. Создание массивов объектов
2. Повторение элементов с трансформациями
3. Создание симметричных копий
4. Масштабирование и вращение объектов
5. Создание сложных композиций из простых элементов

## Интеграция с другими объектами

- Использует любые Construction объекты как источник
- Может быть источником для других CopyConstruction
- Может использоваться как база для SymmetryConstruction
- Может быть частью PathConstruction
- Может использоваться как ограничитель для других геометрических объектов

## Примеры использования

### Базовое использование

```csharp
// Создание простой копии объекта
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 50, 50), 10);

CopyConstruction copy = new CopyConstruction(document);
copy.SetSource(originalCircle);
copy.SetTranslation(30, 0, 0); // Смещение вправо на 30 единиц
copy.Color = 255; // Красный цвет
```

### Создание копии с вращением

```csharp
// Создание копии с вращением
LineConstruction originalLine = new LineConstruction(document);
originalLine.SetTwoNodes(new FreeNode(document, 40, 50), new FreeNode(document, 60, 50));

CopyConstruction rotatedCopy = new CopyConstruction(document);
rotatedCopy.SetSource(originalLine);
// Вращение на 45 градусов вокруг центра (50, 50)
rotatedCopy.SetRotation(Math.PI / 4, 50, 50, 0);
rotatedCopy.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание массива копий

```csharp
// Создание массива копий
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 30, 50), 5);

int arrayCount = 5;
CopyConstruction[] copies = new CopyConstruction[arrayCount];

for (int i = 0; i < arrayCount; i++)
{
    copies[i] = new CopyConstruction(document);
    copies[i].SetSource(originalCircle);
    copies[i].SetTranslation(i * 15, 0, 0); // Смещение по X
    
    // Установка цвета с градиентом
    int red = (int)(255 * (double)i / (arrayCount - 1));
    int green = 255 - red;
    int blue = 128;
    copies[i].Color = (red << 16) | (green << 8) | blue;
}
```

### Создание копий с геометрическими трансформациями

```csharp
// Создание копий с различными трансформациями
EllipseConstruction originalEllipse = new EllipseConstruction(document);
originalEllipse.SetCenterAndRadii(new FreeNode(document, 50, 50), 15, 10);

int transformCount = 4;
CopyConstruction[] transformedCopies = new CopyConstruction[transformCount];

for (int i = 0; i < transformCount; i++)
{
    transformedCopies[i] = new CopyConstruction(document);
    transformedCopies[i].SetSource(originalEllipse);
    
    switch (i)
    {
        case 0: // Трансляция
            transformedCopies[i].SetTranslation(40, 0, 0);
            break;
        case 1: // Вращение
            transformedCopies[i].SetRotation(Math.PI / 2, 50, 50, 0);
            break;
        case 2: // Масштабирование
            // В реальной реализации потребуется способ применения масштабирования
            transformedCopies[i].SetTranslation(0, 40, 0);
            break;
        case 3: // Комбинация трансформаций
            transformedCopies[i].SetTranslation(-40, 0, 0);
            // В реальной реализации можно комбинировать трансформации
            break;
    }
    
    // Установка цвета
    transformedCopies[i].Color = 16711680; // Синий цвет
}
```

### Создание параметризованной системы копий

```csharp
// Создание параметризованной системы копий
SplineConstruction originalSpline = new SplineConstruction(document);

// Создание точек сплайна
FreeNode[] splinePoints = new FreeNode[4];
splinePoints[0] = new FreeNode(document, 30, 50);
splinePoints[1] = new FreeNode(document, 40, 40);
splinePoints[2] = new FreeNode(document, 50, 60);
splinePoints[3] = new FreeNode(document, 60, 50);

for (int i = 0; i < 4; i++)
{
    originalSpline.Points.Add(splinePoints[i]);
}

int parametricCount = 6;
CopyConstruction[] parametricCopies = new CopyConstruction[parametricCount];

for (int i = 0; i < parametricCount; i++)
{
    parametricCopies[i] = new CopyConstruction(document);
    parametricCopies[i].SetSource(originalSpline);
    
    // Параметрическое смещение
    double angle = 2 * Math.PI * i / parametricCount;
    double radius = 30;
    double dx = radius * Math.Cos(angle);
    double dy = radius * Math.Sin(angle);
    parametricCopies[i].SetTranslation(dx, dy, 0);
    
    // Параметрическое вращение
    parametricCopies[i].SetRotation(angle, 50, 50, 0);
    
    // Установка цвета
    int red = (int)(255 * (1 + Math.Cos(angle)) / 2);
    int green = (int)(255 * (1 + Math.Sin(angle)) / 2);
    int blue = (int)(255 * (1 + Math.Cos(angle + Math.PI / 3)) / 2);
    parametricCopies[i].Color = (red << 16) | (green << 8) | blue;
}
```

### Интеграция с другими объектами

```csharp
// Создание копий, интегрированных с другими объектами
PathConstruction originalPath = new PathConstruction(document);

// Создание контура
FreeNode[] pathNodes = new FreeNode[4];
pathNodes[0] = new FreeNode(document, 40, 40);
pathNodes[1] = new FreeNode(document, 60, 40);
pathNodes[2] = new FreeNode(document, 60, 60);
pathNodes[3] = new FreeNode(document, 40, 60);

for (int i = 0; i < 4; i++)
{
    originalPath.AddSegment(pathNodes[i], pathNodes[(i + 1) % 4]);
}

// Создание копий контура
int pathCopyCount = 4;
CopyConstruction[] pathCopies = new CopyConstruction[pathCopyCount];

for (int i = 0; i < pathCopyCount; i++)
{
    pathCopies[i] = new CopyConstruction(document);
    pathCopies[i].SetSource(originalPath);
    pathCopies[i].SetTranslation(i * 25, i * 25, 0);
    pathCopies[i].Color = 16776960; // Желтый цвет
}

// Создание вспомогательных линий между оригиналом и копиями
LineConstruction[] helperLines = new LineConstruction[pathCopyCount];
for (int i = 0; i < pathCopyCount; i++)
{
    helperLines[i] = new LineConstruction(document);
    helperLines[i].SetTwoNodes(
        new FreeNode(document, 50, 50),
        new FreeNode(document, 50 + i * 25, 50 + i * 25));
    helperLines[i].Color = 12632256; // Серый цвет
    helperLines[i].Style = LineStyle.Dash;
}
```

### Оптимизация производительности

```csharp
// Создание большого количества копий с оптимизацией
int copyCount = 100;
CopyConstruction[] copies = new CopyConstruction[copyCount];
CircleConstruction[] sourceCircles = new CircleConstruction[10];

// Создание небольшого количества исходных объектов
for (int i = 0; i < 10; i++)
{
    sourceCircles[i] = new CircleConstruction(document);
    sourceCircles[i].SetCenterAndRadius(
        new FreeNode(document, 30 + i * 10, 50), 3);
}

// Создание копий с использованием ограниченного набора источников
for (int i = 0; i < copyCount; i++)
{
    copies[i] = new CopyConstruction(document);
    copies[i].SetSource(sourceCircles[i % 10]);
    copies[i].SetTranslation((i % 10) * 15, (i / 10) * 15, 0);
    // Установка цвета
    copies[i].Color = (i * 10) % 256;
}
```

### Работа с динамическими копиями

```csharp
// Создание динамической копии
CircleConstruction dynamicSource = new CircleConstruction(document);
dynamicSource.SetCenterAndRadius(new FreeNode(document, 50, 50), 10);

CopyConstruction dynamicCopy = new CopyConstruction(document);
dynamicCopy.SetSource(dynamicSource);
dynamicCopy.SetTranslation(30, 0, 0);
dynamicCopy.Color = 16711680; // Синий цвет

// В реальном приложении здесь могла бы быть логика обновления свойств копии
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicCopy(double time)
{
    // Обновление трансляции
    double dx = 30 + 20 * Math.Sin(time * 0.5);
    double dy = 20 * Math.Cos(time * 0.5);
    dynamicCopy.SetTranslation(dx, dy, 0);
    
    // Обновление вращения
    dynamicCopy.SetRotation(time, 50, 50, 0);
    
    // Обновление цвета
    int red = (int)(255 * (1 + Math.Sin(time)) / 2);
    int green = (int)(255 * (1 + Math.Cos(time + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(time + 2 * Math.PI / 3)) / 2);
    dynamicCopy.Color = (red << 16) | (green << 8) | blue;
}
*/
```

## Связанные концепции

- SymmetryConstruction - Симметричная копия линии построения
- OffsetConstruction - Смещенная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура
- Matrix3D - Трехмерная матрица трансформации

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества копий
2. Используйте параметризованные копии для создания динамических конструкций
3. При создании больших массивов копий используйте оптимизацию производительности
4. Убедитесь, что исходные объекты существуют и корректны
5. Используйте копии повторно при создании сложных конструкций
6. Проверяйте трансформации перед применением к копиям

## Математические аспекты

- Трансформации применяются через матричные операции
- Трансляции, вращения и масштабирования комбинируются через матричное умножение
- Геометрические преобразования вычисляются с использованием линейной алгебры
- Точки трансформируются через умножение на матрицу трансформации

## Совместимость и ограничения

- CopyConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях
- Ограничения связаны с диапазоном допустимых значений трансформаций
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- CopyConstruction может быть расширен через наследование для создания специализированных типов копий
- Может быть интегрирован с пользовательскими математическими функциями трансформации
- Поддерживает пользовательские свойства через механизм параметров T-Flex
# OffsetConstruction - примеры использования

Класс `OffsetConstruction` представляет линию построения-эквидистанту. Этот класс наследуется от `Construction` и предоставляет специфичные свойства и методы для создания эквидистантных линий построения.

## Основные свойства

- `Source` - Исходная линия построения
- `Offset` - Смещение эквидистанты
- `OffsetNode` - Узел, задающий смещение
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения

## Примеры использования

### 1. Создание эквидистанты для окружности

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание эквидистанты для окружности");

// Создание исходной окружности
CircleConstruction circle = new CircleConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
circle.SetCenterAndRadius(center, 20);

// Создание эквидистанты
OffsetConstruction offsetCircle = new OffsetConstruction(document);
offsetCircle.Source = circle;
offsetCircle.Offset = 10; // Смещение на 10 единиц

// Установка визуальных свойств
offsetCircle.Color = 255; // Красный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание эквидистанты с использованием узла смещения

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание эквидистанты с узлом смещения");

// Создание исходного эллипса
EllipseConstruction ellipse = new EllipseConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
FreeNode major = new FreeNode(document, 70, 50);
FreeNode minor = new FreeNode(document, 50, 60);
ellipse.SetCenterAndTwoNodes(center, major, minor);

// Создание узла для задания смещения
FreeNode offsetNode = new FreeNode(document, 50, 80);

// Создание эквидистанты
OffsetConstruction offsetEllipse = new OffsetConstruction(document);
offsetEllipse.Source = ellipse;
offsetEllipse.OffsetNode = offsetNode;

// Установка визуальных свойств
offsetEllipse.Color = 65280; // Зеленый цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание эквидистанты для линии

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание эквидистанты для линии");

// Создание исходной линии
LineConstruction line = new LineConstruction(document);
FreeNode start = new FreeNode(document, 10, 10);
FreeNode end = new FreeNode(document, 50, 30);
line.SetTwoNodes(start, end);

// Создание эквидистанты
OffsetConstruction offsetLine = new OffsetConstruction(document);
offsetLine.Source = line;
offsetLine.Offset = 5; // Смещение на 5 единиц

// Установка визуальных свойств
offsetLine.Color = 16711680; // Синий цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Создание эквидистанты для сплайна

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание эквидистанты для сплайна");

// Создание исходного сплайна
SplineConstruction spline = new SplineConstruction(document);
// Добавление точек сплайна
spline.Points.Add(new FreeNode(document, 10, 10));
spline.Points.Add(new FreeNode(document, 30, 20));
spline.Points.Add(new FreeNode(document, 50, 15));
spline.Points.Add(new FreeNode(document, 70, 25));

// Создание эквидистанты
OffsetConstruction offsetSpline = new OffsetConstruction(document);
offsetSpline.Source = spline;
offsetSpline.Offset = 8; // Смещение на 8 единиц

// Установка визуальных свойств
offsetSpline.Color = 16711935; // Пурпурный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Создание нескольких эквидистант с разным смещением

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание нескольких эквидистант");

// Создание исходной окружности
CircleConstruction circle = new CircleConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
circle.SetCenterAndRadius(center, 15);

// Создание нескольких эквидистант с разным смещением
double[] offsets = { 5, 10, 15, 20 };
int[] colors = { 255, 65280, 16711680, 16776960 };

for (int i = 0; i < offsets.Length; i++)
{
    OffsetConstruction offsetCircle = new OffsetConstruction(document);
    offsetCircle.Source = circle;
    offsetCircle.Offset = offsets[i];
    offsetCircle.Color = colors[i];
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Интеграция эквидистант с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция эквидистант с другими объектами");

// Создание исходного эллипса
EllipseConstruction ellipse = new EllipseConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
FreeNode major = new FreeNode(document, 70, 50);
FreeNode minor = new FreeNode(document, 50, 60);
ellipse.SetCenterAndTwoNodes(center, major, minor);

// Создание эквидистанты
OffsetConstruction offsetEllipse = new OffsetConstruction(document);
offsetEllipse.Source = ellipse;
offsetEllipse.Offset = 10;

// Создание линии, соединяющей центр исходного эллипса с центром эквидистанты
// Для этого нужно получить центр эквидистанты (в данном случае он совпадает с центром исходного эллипса)
LineConstruction connectionLine = new LineConstruction(document);
connectionLine.SetTwoNodes(center, new FreeNode(document, center.X.Value + 15, center.Y.Value));

// Установка визуальных свойств
ellipse.Color = 255; // Красный (исходный эллипс)
offsetEllipse.Color = 65280; // Зеленый (эквидистанта)
connectionLine.Color = 16711680; // Синий (соединительная линия)

// Закрытие блока изменений документа
document.EndChanges();
```

## Свойства и методы

### Основные свойства:

- `Source` - Исходная линия построения
- `Offset` - Смещение эквидистанты
- `OffsetNode` - Узел, задающий смещение
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения

### Унаследованные свойства от Construction:

- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым

## Заключение

Класс `OffsetConstruction` предоставляет удобные средства для создания эквидистантных линий построения в T-Flex CAD. Он поддерживает различные типы исходных объектов (окружности, эллипсы, линии, сплайны и др.) и позволяет задавать смещение как числовым значением, так и с помощью узла. Эквидистанты могут быть использованы для создания концентрических конструкций, параллельных линий и других геометрических элементов.
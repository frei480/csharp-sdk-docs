# SymmetryConstruction - примеры использования

Класс `SymmetryConstruction` представляет линию построения, симметричную относительно оси. Этот класс наследуется от `Construction` и предоставляет специфичные свойства и методы для создания симметричных копий объектов.

## Основные свойства

- `Source` - Исходная линия построения
- `Axis` - Ось симметрии
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения

## Примеры использования

### 1. Создание симметрии относительно вертикальной оси

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание симметрии относительно вертикальной оси");

// Создание исходной линии построения (например, треугольника из линий)
LineConstruction line1 = new LineConstruction(document);
LineConstruction line2 = new LineConstruction(document);
LineConstruction line3 = new LineConstruction(document);

// Создание узлов для треугольника
FreeNode node1 = new FreeNode(document, 30, 30);
FreeNode node2 = new FreeNode(document, 50, 50);
FreeNode node3 = new FreeNode(document, 10, 50);

// Построение треугольника
line1.SetTwoNodes(node1, node2);
line2.SetTwoNodes(node2, node3);
line3.SetTwoNodes(node3, node1);

// Создание оси симметрии (вертикальная линия посередине)
LineConstruction axis = new LineConstruction(document);
FreeNode axisStart = new FreeNode(document, 30, 10);
FreeNode axisEnd = new FreeNode(document, 30, 70);
axis.SetTwoNodes(axisStart, axisEnd);

// Создание симметричной копии
SymmetryConstruction symmetry = new SymmetryConstruction(document);
symmetry.Source = line1; // Можно указать любую из линий или создать контур
symmetry.Axis = axis;

// Установка визуальных свойств
symmetry.Color = 255; // Красный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание симметрии для окружности

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание симметрии для окружности");

// Создание исходной окружности
CircleConstruction circle = new CircleConstruction(document);
FreeNode center = new FreeNode(document, 50, 50);
circle.SetCenterAndRadius(center, 15);

// Создание оси симметрии (горизонтальная линия)
LineConstruction axis = new LineConstruction(document);
FreeNode axisStart = new FreeNode(document, 10, 50);
FreeNode axisEnd = new FreeNode(document, 90, 50);
axis.SetTwoNodes(axisStart, axisEnd);

// Создание симметричной копии
SymmetryConstruction symmetryCircle = new SymmetryConstruction(document);
symmetryCircle.Source = circle;
symmetryCircle.Axis = axis;

// Установка визуальных свойств
symmetryCircle.Color = 65280; // Зеленый цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание симметрии для сложного объекта

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание симметрии для сложного объекта");

// Создание сложного объекта (например, прямоугольника с закругленными углами)
// Создание контура прямоугольника
PathConstruction rectangle = new PathConstruction(document);

// Создание узлов для прямоугольника
FreeNode[] nodes = new FreeNode[4];
nodes[0] = new FreeNode(document, 20, 20);
nodes[1] = new FreeNode(document, 60, 20);
nodes[2] = new FreeNode(document, 60, 50);
nodes[3] = new FreeNode(document, 20, 50);

// Добавление сегментов в контур
rectangle.AddSegment(nodes[0], nodes[1]);
rectangle.AddSegment(nodes[1], nodes[2]);
rectangle.AddSegment(nodes[2], nodes[3]);
rectangle.AddSegment(nodes[3], nodes[0]);

// Создание оси симметрии (вертикальная линия посередине прямоугольника)
LineConstruction axis = new LineConstruction(document);
FreeNode axisStart = new FreeNode(document, 40, 10);
FreeNode axisEnd = new FreeNode(document, 40, 60);
axis.SetTwoNodes(axisStart, axisEnd);

// Создание симметричной копии
SymmetryConstruction symmetryRectangle = new SymmetryConstruction(document);
symmetryRectangle.Source = rectangle;
symmetryRectangle.Axis = axis;

// Установка визуальных свойств
rectangle.Color = 255; // Красный цвет (исходный прямоугольник)
symmetryRectangle.Color = 65280; // Зеленый цвет (симметричная копия)

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Создание двойной симметрии

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание двойной симметрии");

// Создание исходной линии построения (например, линии)
LineConstruction sourceLine = new LineConstruction(document);
FreeNode startNode = new FreeNode(document, 25, 25);
FreeNode endNode = new FreeNode(document, 35, 35);
sourceLine.SetTwoNodes(startNode, endNode);

// Создание первой оси симметрии (вертикальная)
LineConstruction axis1 = new LineConstruction(document);
FreeNode axis1Start = new FreeNode(document, 30, 10);
FreeNode axis1End = new FreeNode(document, 30, 50);
axis1.SetTwoNodes(axis1Start, axis1End);

// Создание первой симметрии
SymmetryConstruction symmetry1 = new SymmetryConstruction(document);
symmetry1.Source = sourceLine;
symmetry1.Axis = axis1;

// Создание второй оси симметрии (горизонтальная)
LineConstruction axis2 = new LineConstruction(document);
FreeNode axis2Start = new FreeNode(document, 10, 30);
FreeNode axis2End = new FreeNode(document, 50, 30);
axis2.SetTwoNodes(axis2Start, axis2End);

// Создание второй симметрии от первой симметрии
SymmetryConstruction symmetry2 = new SymmetryConstruction(document);
symmetry2.Source = symmetry1;
symmetry2.Axis = axis2;

// Установка визуальных свойств
sourceLine.Color = 255; // Красный цвет (исходная линия)
symmetry1.Color = 65280; // Зеленый цвет (первая симметрия)
symmetry2.Color = 16711680; // Синий цвет (вторая симметрия)

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Создание симметрии с использованием существующих объектов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание симметрии с использованием существующих объектов");

// Предположим, у нас есть уже созданные объекты в документе
// Найдем их по имени или другим критериям
// Construction existingObject = document.Constructions.FindByName("ИсходныйОбъект");
// LineConstruction existingAxis = document.Constructions.FindByType(ConstructionType.Line).FirstOrDefault() as LineConstruction;

// Для примера создадим объекты явно
EllipseConstruction ellipse = new EllipseConstruction(document);
FreeNode center = new FreeNode(document, 40, 40);
FreeNode major = new FreeNode(document, 60, 40);
FreeNode minor = new FreeNode(document, 40, 50);
ellipse.SetCenterAndTwoNodes(center, major, minor);

// Создание оси симметрии под углом 45 градусов
LineConstruction axis = new LineConstruction(document);
FreeNode axisStart = new FreeNode(document, 20, 20);
FreeNode axisEnd = new FreeNode(document, 60, 60);
axis.SetTwoNodes(axisStart, axisEnd);

// Создание симметричной копии
SymmetryConstruction symmetryEllipse = new SymmetryConstruction(document);
symmetryEllipse.Source = ellipse;
symmetryEllipse.Axis = axis;

// Установка визуальных свойств
ellipse.Color = 255; // Красный цвет (исходный эллипс)
symmetryEllipse.Color = 16711935; // Пурпурный цвет (симметричная копия)

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Интеграция симметрии с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция симметрии с другими объектами");

// Создание исходного объекта (например, сплайна)
SplineConstruction spline = new SplineConstruction(document);
// Добавление точек сплайна
spline.Points.Add(new FreeNode(document, 20, 30));
spline.Points.Add(new FreeNode(document, 30, 40));
spline.Points.Add(new FreeNode(document, 40, 35));
spline.Points.Add(new FreeNode(document, 50, 45));

// Создание оси симметрии (горизонтальная линия)
LineConstruction axis = new LineConstruction(document);
FreeNode axisStart = new FreeNode(document, 10, 40);
FreeNode axisEnd = new FreeNode(document, 70, 40);
axis.SetTwoNodes(axisStart, axisEnd);

// Создание симметричной копии
SymmetryConstruction symmetrySpline = new SymmetryConstruction(document);
symmetrySpline.Source = spline;
symmetrySpline.Axis = axis;

// Создание линии, соединяющей соответствующие точки исходного сплайна и симметричной копии
// Для примера соединим первую точку исходного сплайна с первой точкой симметричной копии
// В реальности для получения точек симметричного объекта может потребоваться дополнительная логика
LineConstruction connectionLine = new LineConstruction(document);
connectionLine.SetTwoNodes(spline.Points[0], new FreeNode(document, spline.Points[0].X.Value, 80 - spline.Points[0].Y.Value));

// Установка визуальных свойств
spline.Color = 255; // Красный цвет (исходный сплайн)
symmetrySpline.Color = 65280; // Зеленый цвет (симметричная копия)
connectionLine.Color = 16711680; // Синий цвет (соединительная линия)

// Закрытие блока изменений документа
document.EndChanges();
```

## Свойства и методы

### Основные свойства:

- `Source` - Исходная линия построения
- `Axis` - Ось симметрии
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения

### Унаследованные свойства от Construction:

- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым

## Заключение

Класс `SymmetryConstruction` предоставляет удобные средства для создания симметричных копий объектов в T-Flex CAD. Он позволяет создавать симметричные копии относительно заданной оси, что полезно при построении симметричных геометрических конструкций. Симметричные объекты сохраняют ассоциативную связь с исходными объектами и осью симметрии, что позволяет автоматически обновлять симметричные копии при изменении исходных объектов.
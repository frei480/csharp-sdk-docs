# SymmetryConstruction - База знаний для RAG-системы

## Общее описание

SymmetryConstruction представляет собой симметричную линию построения в T-Flex CAD API. Это геометрический элемент для создания симметричных копий других геометрических объектов относительно заданной оси.

## Основные характеристики

- Тип: Симметричная линия построения
- Назначение: Создание симметричных копий геометрических объектов
- Использование: Создание симметричных конструкций, зеркальных копий, симметричных массивов
- Связь с другими объектами: Использует другие геометрические объекты как источник и линию как ось симметрии

## Конструкторы

1. `SymmetryConstruction(Document doc)` - Создает пустую симметричную линию построения

## Свойства

- `Source` - Исходная линия построения (Construction)
- `Axis` - Ось симметрии (LineConstruction)
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
- `SetAxis(LineConstruction axis)` - Установка оси симметрии
- `GetSymmetricGeometry()` - Получение симметричной геометрии
- `GetReflectionMatrix()` - Получение матрицы отражения

## Паттерны использования

1. Создание симметричных конструкций
2. Создание зеркальных копий объектов
3. Генерация симметричных массивов
4. Создание симметричных контуров
5. Построение симметричных композиций

## Интеграция с другими объектами

- Использует любые Construction объекты как источник
- Использует LineConstruction как ось симметрии
- Может быть источником для других SymmetryConstruction
- Может использоваться как база для CopyConstruction
- Может быть частью PathConstruction

## Примеры использования

### Базовое использование

```csharp
// Создание простой симметрии
LineConstruction originalLine = new LineConstruction(document);
originalLine.SetTwoNodes(new FreeNode(document, 30, 40), new FreeNode(document, 50, 60));

// Создание оси симметрии (вертикальная линия)
LineConstruction symmetryAxis = new LineConstruction(document);
symmetryAxis.SetTwoNodes(new FreeNode(document, 40, 30), new FreeNode(document, 40, 70));

SymmetryConstruction symmetry = new SymmetryConstruction(document);
symmetry.SetSource(originalLine);
symmetry.SetAxis(symmetryAxis);
symmetry.Color = 255; // Красный цвет
```

### Создание симметрии контура

```csharp
// Создание симметрии замкнутого контура
PathConstruction originalPath = new PathConstruction(document);

// Создание треугольного контура
FreeNode[] nodes = new FreeNode[3];
nodes[0] = new FreeNode(document, 30, 30);
nodes[1] = new FreeNode(document, 50, 30);
nodes[2] = new FreeNode(document, 40, 50);

for (int i = 0; i < 3; i++)
{
    originalPath.AddSegment(nodes[i], nodes[(i + 1) % 3]);
}

// Создание оси симметрии (вертикальная линия через центр)
LineConstruction symmetryAxis = new LineConstruction(document);
symmetryAxis.SetTwoNodes(new FreeNode(document, 40, 20), new FreeNode(document, 40, 60));

SymmetryConstruction pathSymmetry = new SymmetryConstruction(document);
pathSymmetry.SetSource(originalPath);
pathSymmetry.SetAxis(symmetryAxis);
pathSymmetry.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание множественных симметрий

```csharp
// Создание множественных симметрий
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 30, 50), 10);

int symmetryCount = 4;
SymmetryConstruction[] symmetries = new SymmetryConstruction[symmetryCount];
LineConstruction[] symmetryAxes = new LineConstruction[symmetryCount];

for (int i = 0; i < symmetryCount; i++)
{
    symmetries[i] = new SymmetryConstruction(document);
    symmetries[i].SetSource(originalCircle);
    
    // Создание осей симметрии под разными углами
    double angle = Math.PI * i / symmetryCount;
    double axisStartX = 50 - 30 * Math.Cos(angle);
    double axisStartY = 50 - 30 * Math.Sin(angle);
    double axisEndX = 50 + 30 * Math.Cos(angle);
    double axisEndY = 50 + 30 * Math.Sin(angle);
    
    FreeNode axisStart = new FreeNode(document, axisStartX, axisStartY);
    FreeNode axisEnd = new FreeNode(document, axisEndX, axisEndY);
    symmetryAxes[i] = new LineConstruction(document);
    symmetryAxes[i].SetTwoNodes(axisStart, axisEnd);
    symmetryAxes[i].Color = 12632256; // Серый цвет
    symmetryAxes[i].Style = LineStyle.Dash;
    
    symmetries[i].SetAxis(symmetryAxes[i]);
    
    // Установка цвета с градиентом
    int red = (int)(255 * (double)i / (symmetryCount - 1));
    int green = 255 - red;
    int blue = 128;
    symmetries[i].Color = (red << 16) | (green << 8) | blue;
}
```

### Создание симметрий с геометрическими расчетами

```csharp
// Создание симметрий с геометрическими расчетами
SplineConstruction originalSpline = new SplineConstruction(document);

// Создание точек сплайна в форме волны
int pointCount = 8;
for (int i = 0; i < pointCount; i++)
{
    double x = 20 + i * 5;
    double y = 50 + 10 * Math.Sin(i * 0.5);
    FreeNode point = new FreeNode(document, x, y);
    originalSpline.Points.Add(point);
}

// Создание симметрии относительно горизонтальной оси
LineConstruction horizontalAxis = new LineConstruction(document);
horizontalAxis.SetTwoNodes(new FreeNode(document, 20, 50), new FreeNode(document, 60, 50));

SymmetryConstruction splineSymmetry = new SymmetryConstruction(document);
splineSymmetry.SetSource(originalSpline);
splineSymmetry.SetAxis(horizontalAxis);
splineSymmetry.Color = 16711680; // Синий цвет
```

### Создание параметризованной системы симметрий

```csharp
// Создание параметризованной системы симметрий
EllipseConstruction originalEllipse = new EllipseConstruction(document);
originalEllipse.SetCenterAndRadii(new FreeNode(document, 50, 50), 20, 12);

int parametricCount = 6;
SymmetryConstruction[] parametricSymmetries = new SymmetryConstruction[parametricCount];
LineConstruction[] parametricAxes = new LineConstruction[parametricCount];

for (int i = 0; i < parametricCount; i++)
{
    parametricSymmetries[i] = new SymmetryConstruction(document);
    parametricSymmetries[i].SetSource(originalEllipse);
    
    // Создание осей симметрии под параметрическими углами
    double angle = 2 * Math.PI * i / parametricCount;
    double axisLength = 30;
    double axisStartX = 50 - axisLength * Math.Cos(angle);
    double axisStartY = 50 - axisLength * Math.Sin(angle);
    double axisEndX = 50 + axisLength * Math.Cos(angle);
    double axisEndY = 50 + axisLength * Math.Sin(angle);
    
    FreeNode axisStart = new FreeNode(document, axisStartX, axisStartY);
    FreeNode axisEnd = new FreeNode(document, axisEndX, axisEndY);
    parametricAxes[i] = new LineConstruction(document);
    parametricAxes[i].SetTwoNodes(axisStart, axisEnd);
    parametricAxes[i].Color = 12632256; // Серый цвет
    parametricAxes[i].Style = LineStyle.Dash;
    
    parametricSymmetries[i].SetAxis(parametricAxes[i]);
    
    // Установка цвета
    int red = (int)(255 * (1 + Math.Cos(angle)) / 2);
    int green = (int)(255 * (1 + Math.Sin(angle)) / 2);
    int blue = (int)(255 * (1 + Math.Cos(angle + Math.PI / 3)) / 2);
    parametricSymmetries[i].Color = (red << 16) | (green << 8) | blue;
}
```

### Интеграция с другими объектами

```csharp
// Создание симметрии, интегрированной с другими объектами
PathConstruction originalPath = new PathConstruction(document);

// Создание контура в форме буквы "V"
FreeNode[] vNodes = new FreeNode[3];
vNodes[0] = new FreeNode(document, 40, 60);
vNodes[1] = new FreeNode(document, 50, 30);
vNodes[2] = new FreeNode(document, 60, 60);

for (int i = 0; i < 2; i++)
{
    originalPath.AddSegment(vNodes[i], vNodes[i + 1]);
}

// Создание оси симметрии (вертикальная линия через вершину)
LineConstruction symmetryAxis = new LineConstruction(document);
symmetryAxis.SetTwoNodes(new FreeNode(document, 50, 20), new FreeNode(document, 50, 70));

SymmetryConstruction vSymmetry = new SymmetryConstruction(document);
vSymmetry.SetSource(originalPath);
vSymmetry.SetAxis(symmetryAxis);
vSymmetry.Color = 255; // Красный цвет

// Создание вспомогательных линий
LineConstruction[] helperLines = new LineConstruction[2];
// Линия от левой точки к оси
helperLines[0] = new LineConstruction(document);
helperLines[0].SetTwoNodes(vNodes[0], new FreeNode(document, 50, 60));
helperLines[0].Color = 12632256; // Серый цвет
helperLines[0].Style = LineStyle.DashDot;

// Линия от правой точки к оси
helperLines[1] = new LineConstruction(document);
helperLines[1].SetTwoNodes(vNodes[2], new FreeNode(document, 50, 60));
helperLines[1].Color = 12632256; // Серый цвет
helperLines[1].Style = LineStyle.DashDot;
```

### Оптимизация производительности

```csharp
// Создание большого количества симметрий с оптимизацией
int symmetryCount = 40;
SymmetryConstruction[] symmetries = new SymmetryConstruction[symmetryCount];
LineConstruction[] sourceLines = new LineConstruction[10];
LineConstruction[] symmetryAxes = new LineConstruction[symmetryCount];

// Создание небольшого количества исходных линий
for (int i = 0; i < 10; i++)
{
    sourceLines[i] = new LineConstruction(document);
    sourceLines[i].SetTwoNodes(
        new FreeNode(document, 30 + i * 5, 40), 
        new FreeNode(document, 30 + i * 5, 60));
}

// Создание осей симметрии
for (int i = 0; i < symmetryCount; i++)
{
    double axisX = 20 + (i % 10) * 7;
    symmetryAxes[i] = new LineConstruction(document);
    symmetryAxes[i].SetTwoNodes(
        new FreeNode(document, axisX, 30), 
        new FreeNode(document, axisX, 70));
}

// Создание симметрий с использованием ограниченного набора источников
for (int i = 0; i < symmetryCount; i++)
{
    symmetries[i] = new SymmetryConstruction(document);
    symmetries[i].SetSource(sourceLines[i % 10]);
    symmetries[i].SetAxis(symmetryAxes[i]);
    // Установка цвета
    symmetries[i].Color = (i * 20) % 256;
}
```

### Работа с динамическими симметриями

```csharp
// Создание динамической симметрии
CircleConstruction dynamicSource = new CircleConstruction(document);
dynamicSource.SetCenterAndRadius(new FreeNode(document, 50, 50), 12);

LineConstruction dynamicAxis = new LineConstruction(document);
dynamicAxis.SetTwoNodes(new FreeNode(document, 30, 50), new FreeNode(document, 70, 50));

SymmetryConstruction dynamicSymmetry = new SymmetryConstruction(document);
dynamicSymmetry.SetSource(dynamicSource);
dynamicSymmetry.SetAxis(dynamicAxis);
dynamicSymmetry.Color = 16711680; // Синий цвет

// В реальном приложении здесь могла бы быть логика обновления свойств симметрии
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicSymmetry(double time)
{
    // Обновление центра исходной окружности
    dynamicSource.Center.X.Value = 50 + 10 * Math.Sin(time * 0.5);
    dynamicSource.Center.Y.Value = 50 + 10 * Math.Cos(time * 0.5);
    
    // Обновление оси симметрии
    double axisOffset = 5 * Math.Sin(time * 0.3);
    dynamicAxis.Node1.Y.Value = 50 + axisOffset;
    dynamicAxis.Node2.Y.Value = 50 + axisOffset;
    
    // Обновление цвета
    int red = (int)(255 * (1 + Math.Sin(time)) / 2);
    int green = (int)(255 * (1 + Math.Cos(time + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(time + 2 * Math.PI / 3)) / 2);
    dynamicSymmetry.Color = (red << 16) | (green << 8) | blue;
}
*/
```

## Связанные концепции

- CopyConstruction - Копия линии построения
- OffsetConstruction - Смещенная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- LineConstruction - Линия построения
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества симметрий
2. Используйте параметризованные симметрии для создания динамических конструкций
3. При создании больших массивов симметрий используйте оптимизацию производительности
4. Убедитесь, что исходные объекты и оси симметрии существуют и корректны
5. Проверяйте геометрические свойства симметрий перед использованием в сложных расчетах
6. Используйте симметрии повторно при создании сложных конструкций

## Математические аспекты

- Симметрии вычисляются через отражение относительно оси
- Матрица отражения вычисляется на основе уравнения оси симметрии
- Точки симметричной копии вычисляются через матричные операции
- Расстояния от точек до оси симметрии сохраняются

## Совместимость и ограничения

- SymmetryConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях
- Ограничения связаны с геометрической сложностью исходных объектов
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- SymmetryConstruction может быть расширен через наследование для создания специализированных типов симметрий
- Может быть интегрирован с пользовательскими математическими функциями вычисления отражений
- Поддерживает пользовательские свойства через механизм параметров T-Flex
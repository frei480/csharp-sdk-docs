# CopyConstruction - примеры использования

Класс `CopyConstruction` представляет линию построения, полученную ассоциативным копированием. Этот класс наследуется от `Construction` и предоставляет специфичные свойства и методы для работы с копиями объектов.

## Основные свойства

- `Source` - Исходная линия построения
- `SourceCopyOperation` - Исходный объект-копия
- `Transformation` - Преобразование
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения

## Примеры использования

### 1. Создание копии линии построения

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание копии линии построения");

// Создание исходной линии построения (например, линии)
LineConstruction sourceLine = new LineConstruction(document);
FreeNode startNode = new FreeNode(document, 10, 10);
FreeNode endNode = new FreeNode(document, 50, 50);
sourceLine.SetTwoNodes(startNode, endNode);

// Создание копии линии построения
CopyConstruction copyLine = new CopyConstruction(document);
copyLine.Source = sourceLine;
copyLine.Transformation = new Matrix2D(); // Матрица преобразования (по умолчанию - без преобразования)

// Установка визуальных свойств
copyLine.Color = 255; // Красный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание копии с преобразованием

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание копии с преобразованием");

// Создание исходной линии построения (например, окружности)
CircleConstruction sourceCircle = new CircleConstruction(document);
FreeNode centerNode = new FreeNode(document, 50, 50);
sourceCircle.SetCenterAndRadius(centerNode, 20);

// Создание матрицы преобразования (перемещение на 30 единиц по X и 40 по Y)
Matrix2D transform = new Matrix2D();
transform.Translate(30, 40);

// Создание копии с преобразованием
CopyConstruction copyCircle = new CopyConstruction(document);
copyCircle.Source = sourceCircle;
copyCircle.Transformation = transform;

// Установка визуальных свойств
copyCircle.Color = 65280; // Зеленый цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание копии с использованием существующего объекта-копии

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание копии с использованием существующего объекта-копии");

// Создание исходной линии построения (например, эллипса)
EllipseConstruction sourceEllipse = new EllipseConstruction(document);
FreeNode centerNode = new FreeNode(document, 50, 50);
FreeNode majorNode = new FreeNode(document, 70, 50);
FreeNode minorNode = new FreeNode(document, 50, 60);
sourceEllipse.SetCenterAndTwoNodes(centerNode, majorNode, minorNode);

// Предположим, что у нас уже есть объект-копия (например, из операции копирования)
// CopyConstruction existingCopy = ...; // Существующий объект-копия

// Создание новой копии на основе существующего объекта-копии
CopyConstruction newCopy = new CopyConstruction(document);
newCopy.SourceCopyOperation = existingCopy; // Использование существующего объекта-копии

// Установка визуальных свойств
newCopy.Color = 16711680; // Синий цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Работа с копиями в контексте массивов

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание массива копий");

// Создание исходной линии построения (например, прямоугольника)
// Для простоты примера используем линию
LineConstruction sourceLine = new LineConstruction(document);
FreeNode startNode = new FreeNode(document, 10, 10);
FreeNode endNode = new FreeNode(document, 30, 10);
sourceLine.SetTwoNodes(startNode, endNode);

// Создание массива копий с равномерным смещением
int copiesCount = 5;
double offsetX = 10;
double offsetY = 0;

for (int i = 1; i <= copiesCount; i++)
{
    // Создание матрицы преобразования для текущей копии
    Matrix2D transform = new Matrix2D();
    transform.Translate(i * offsetX, i * offsetY);
    
    // Создание копии
    CopyConstruction copy = new CopyConstruction(document);
    copy.Source = sourceLine;
    copy.Transformation = transform;
    
    // Установка визуальных свойств (разные цвета для каждой копии)
    copy.Color = i * 50; // Разные оттенки
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Интеграция с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция копий с другими объектами");

// Создание исходной линии построения
CircleConstruction sourceCircle = new CircleConstruction(document);
FreeNode centerNode = new FreeNode(document, 50, 50);
sourceCircle.SetCenterAndRadius(centerNode, 15);

// Создание копии
CopyConstruction copyCircle = new CopyConstruction(document);
copyCircle.Source = sourceCircle;
Matrix2D transform = new Matrix2D();
transform.Translate(40, 0);
copyCircle.Transformation = transform;

// Создание линии, соединяющей центры исходной окружности и копии
FreeNode copyCenter = new FreeNode(document, centerNode.X.Value + 40, centerNode.Y.Value);
LineConstruction connectionLine = new LineConstruction(document);
connectionLine.SetTwoNodes(centerNode, copyCenter);

// Установка визуальных свойств
copyCircle.Color = 255; // Красный
connectionLine.Color = 65280; // Зеленый

// Закрытие блока изменений документа
document.EndChanges();
```

## Свойства и методы

### Основные свойства:

- `Source` - Исходная линия построения
- `SourceCopyOperation` - Исходный объект-копия
- `Transformation` - Преобразование
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения

### Унаследованные свойства от Construction:

- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым

## Заключение

Класс `CopyConstruction` предоставляет мощные возможности для создания ассоциативных копий объектов в T-Flex CAD. Он поддерживает различные типы преобразований и может быть использован для создания сложных геометрических конструкций, массивов и других повторяющихся элементов. При использовании этого класса важно учитывать, что объекты создаются автоматически системой при создании операции копирования или массива.
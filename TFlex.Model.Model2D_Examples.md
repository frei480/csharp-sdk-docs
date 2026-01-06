# Примеры использования классов в пространстве имён TFlex.Model.Model2D

## Описание пространства имён

Пространство имён `TFlex.Model.Model2D` содержит классы для работы с двумерными объектами в T-Flex CAD, включая проекции, узлы и размеры.

## Основные классы

### Projection

Базовый класс для проекций 3D-моделей на 2D-плоскость.

**Пример создания простой проекции:**
```csharp
Document document = TFlex.Application.ActiveDocument;
document.BeginChanges("Создание проекции");

// Создание простой проекции
SimpleDrawingProjection projection = new SimpleDrawingProjection(document);

// Добавление тела операции
Operation operation = modelObject as Operation;
projection.AddBody(operation);

// Установка типа вида
projection.SetViewType(ProjectionViewType.Front);

// Установка масштаба
projection.Scale = new Parameter(2.0);

// Позиционирование на листе
double posX = (document.ActivePage.Right.Value - document.ActivePage.Left.Value) / 2;
double posY = (document.ActivePage.Top.Value - document.ActivePage.Bottom.Value) / 2;
projection.SetTiePoint(posX, posY);

document.EndChanges();
```

### SimpleDrawingProjection

Класс для создания простых проекций моделей.

**Пример с рабочей плоскостью:**
```csharp
// Создание проекции
SimpleDrawingProjection projection = new SimpleDrawingProjection(document);
projection.AddBody(operation);

// Создание рабочей плоскости
LCSWorkplane workplane = new LCSWorkplane(document);
workplane.LCS = lcs;

// Установка рабочей плоскости вида
projection.SetViewWorkplane(workplane);
```

### FreeNode

Класс для свободных узлов в 2D-пространстве.

**Пример создания узла:**
```csharp
// Создание свободного узла
FreeNode node = new FreeNode(document);
node.X = 100.0;
node.Y = 50.0;

// Или с конструктором
FreeNode centerNode = new FreeNode(document, 25, 25);
```

**Пример использования в размерах:**
```csharp
// Создание узлов для размера
FreeNode node1 = new FreeNode(document);
node1.X = x * scale + posX;
node1.Y = y + posY;

FreeNode node2 = new FreeNode(document);
node2.X = (x - stepLength) * scale + posX;
node2.Y = y + posY;
```

### LinearDimension

Класс для линейных размеров в 2D.

**Пример создания размера между узлами:**
```csharp
// Создание линейного размера
LinearDimension dimension = new LinearDimension(document);

// Установка элементов размера
dimension.SetTwoNodes(node1, node2, DimensionAlignType.Horizontal);

// Установка отступов (горизонтальный, вертикальный, дополнительный)
dimension.SetOffsets(null, offset, null, 0, null, 0);

// Установка типа значения
dimension.ValueType = DimensionValueType.Manual;
dimension.Value = stepLength;
```

**Пример размера по всей длине:**
```csharp
// Размер общей длины
LinearDimension lengthDimension = new LinearDimension(document);
lengthDimension.SetTwoNodes(beginNode, endNode, DimensionAlignType.Horizontal);
lengthDimension.SetOffsets(null, totalOffset, null, 0, null, 0);
lengthDimension.ValueType = DimensionValueType.Manual;
lengthDimension.Value = shaftLength;
```

### DimensionAlignType

Перечисление для типов выравнивания размеров.

**Примеры использования:**
```csharp
// Горизонтальный размер
dimension.SetTwoNodes(node1, node2, DimensionAlignType.Horizontal);

// Вертикальный размер
dimension.SetTwoNodes(node1, node2, DimensionAlignType.Vertical);

// Параллельный размер
dimension.SetTwoNodes(node1, node2, DimensionAlignType.Parallel);
```

### DimensionValueType

Перечисление для типов значений размеров.

**Примеры:**
```csharp
// Ручное значение
dimension.ValueType = DimensionValueType.Manual;
dimension.Value = 50.0;

// Автоматическое значение (расчетное)
dimension.ValueType = DimensionValueType.Auto;

// Значение из параметра
dimension.ValueType = DimensionValueType.Parameter;
dimension.Parameter = someParameter;
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model2D_Examples.md
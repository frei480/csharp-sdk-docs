# Примеры использования классов в пространстве имён TFlex.Model.Model3D

## Описание пространства имён

Пространство имён `TFlex.Model.Model3D` содержит классы для работы с трёхмерными моделями в T-Flex CAD. Оно предоставляет функциональность для создания и манипуляции 3D-объектами, трансформациями, размерами и геометрией.

## Основные классы

### Point3D

Класс для представления точки в 3D-пространстве.

**Пример создания и использования:**
```csharp
// Создание точки
Point3D point = new Point3D(10.0, 20.0, 30.0);

// Получение координат
double x = point.X;
double y = point.Y;
double z = point.Z;

// Изменение координат
point.X = 15.0;
```

### Direction

Класс для представления направления в 3D-пространстве.

**Пример:**
```csharp
// Создание направления
Direction dir = new Direction(1.0, 0.0, 0.0);

// Нормализация
dir.Normalize();

// Получение компонентов
double dx = dir.X;
double dy = dir.Y;
double dz = dir.Z;
```

### AffineTransformation

Класс для аффинных преобразований в 3D-пространстве.

**Пример вращения:**
```csharp
AffineTransformation transform = new AffineTransformation();
ModelAxis axis = new ModelAxis(new Point3D(0, 0, 0), new Direction(0, 0, 1));
transform.Rotate(axis, Math.PI / 2); // Вращение на 90 градусов вокруг Z

Point3D rotatedPoint = originalPoint * transform;
```

### LCS (Local Coordinate System)

Класс для локальной системы координат.

**Пример:**
```csharp
// Создание LCS
LCS lcs = new LCS(document);
lcs.Geometry.Origin = new Point3D(10, 10, 10);
lcs.Geometry.DirectionX = new Direction(1, 0, 0);
lcs.Geometry.DirectionY = new Direction(0, 1, 0);
```

### Node3D

Класс для 3D-узлов в модели.

**Пример получения узла:**
```csharp
Node3D node = Utils.GetNodeByStepIndex(document, stepIndex);
Point3D position = node.Position;
```

### LinearDimension3D

Класс для линейных размеров в 3D.

**Пример создания размера:**
```csharp
LinearDimension3D dimension = new LinearDimension3D(document);
dimension.SetOrientationPlane(workplane);
dimension.SetElements(node1, Dimension3DElementType.Point, node2, Dimension3DElementType.Point, coords);
dimension.SetOffsets(20, 0, 0);
```

### TransformationGroup

Класс для групп трансформаций.

**Пример:**
```csharp
TransformationGroup group = workplane.Transformations.AddBaseTransfGroup();
group.SetLCS(lcs, true);
group.AddRotateTransf(TransformationCoordinate.X, angle);
```

### Parameter

Класс для параметров модели.

**Пример:**
```csharp
Parameter scaleParam = new Parameter(2.0);
projection.Scale = scaleParam;
```

### Operation

Класс для операций модели.

**Пример:**
```csharp
Operation operation = modelObject as Operation;
projection.AddBody(operation);
```

### PointsLCS

Класс для LCS на основе точек.

**Пример:**
```csharp
PointsLCS lcs = new PointsLCS(document) { Name = "MyLCS" };
lcs.PointToOrigin = originPoint;
lcs.DirectionToAxisX = xDirection;
lcs.DirectionToAxisY = yDirection;
```

### LCSWorkplane

Класс для рабочих плоскостей LCS.

**Пример:**
```csharp
LCSWorkplane wp = new LCSWorkplane(document);
wp.LCS = lcs;
```

### DimensionUVCoords

Класс для координат размеров.

**Пример:**
```csharp
DimensionUVCoords coords = new DimensionUVCoords();
// Использование в размерах
```

### ModelAxis

Класс для осей модели.

**Пример:**
```csharp
ModelAxis axis = new ModelAxis(origin, direction);
```

### TransformationCoordinate

Перечисление для координат трансформаций.

**Пример использования:**
```csharp
group.AddMoveTransf(TransformationCoordinate.X, 10.0);
group.AddRotateTransf(TransformationCoordinate.Z, Math.PI);
```

### Dimension3DElementType

Перечисление для типов элементов 3D-размеров.

**Пример:**
```csharp
dimension.SetElements(node1, Dimension3DElementType.Point, node2, Dimension3DElementType.Point, coords);
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D_Examples.md
# Примеры использования классов в пространстве имён TFlex.Model.Model3D.Geometry

## Описание пространства имён

Пространство имён `TFlex.Model.Model3D.Geometry` содержит геометрические примитивы и трансформации для 3D-моделирования.

## Основные классы

### Point3D

**Пример создания и операций:**
```csharp
Point3D origin = new Point3D(0, 0, 0);
Point3D point = new Point3D(10, 20, 30);

// Арифметические операции
Point3D sum = point + new Point3D(5, 5, 5);
Point3D diff = point - origin;
```

### Direction

**Пример работы с направлениями:**
```csharp
Direction xAxis = new Direction(1, 0, 0);
Direction yAxis = new Direction(0, 1, 0);

// Нормализация
xAxis.Normalize();

// Скалярное произведение
double dot = xAxis * yAxis;
```

### Matrix3D

**Пример матричных операций:**
```csharp
Matrix3D identity = Matrix3D.Identity;
Matrix3D transform = new Matrix3D();

// Умножение матриц
Matrix3D result = transform * identity;
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D.Geometry_Examples.md
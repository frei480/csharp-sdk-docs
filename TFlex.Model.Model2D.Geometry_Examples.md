# Примеры использования классов в пространстве имён TFlex.Model.Model2D.Geometry

## Описание пространства имён

Пространство имён `TFlex.Model.Model2D.Geometry` содержит геометрические примитивы для 2D-моделирования.

## Основные классы

### Point2D

Класс для представления точки в 2D-пространстве.

**Пример:**
```csharp
// Создание точки
Point2D point = new Point2D(10.0, 20.0);

// Доступ к координатам
double x = point.X;
double y = point.Y;
```

### Vector2D

Класс для представления вектора в 2D-пространстве.

**Пример:**
```csharp
// Создание вектора
Vector2D vector = new Vector2D(5.0, 3.0);

// Нормализация
vector.Normalize();

// Длина вектора
double length = vector.Length;
```

### Line2D

Класс для представления линии в 2D.

**Пример:**
```csharp
// Создание линии через две точки
Point2D start = new Point2D(0, 0);
Point2D end = new Point2D(10, 10);
Line2D line = new Line2D(start, end);

// Проверка пересечения
Line2D otherLine = new Line2D(new Point2D(0, 10), new Point2D(10, 0));
Point2D intersection = line.Intersect(otherLine);
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model2D.Geometry_Examples.md
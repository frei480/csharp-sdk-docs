# Продвинутые примеры использования классов в пространстве имён TFlex.Model.Model2D.Geometry

## Комплексные геометрические операции

### Булевы операции с 2D-фигурами

```csharp
public void PerformBooleanOperations()
{
    // Создание фигур
    Circle circle1 = new Circle(new Point2D(0, 0), 10);
    Circle circle2 = new Circle(new Point2D(5, 0), 10);
    
    // Объединение
    Region union = circle1.Union(circle2);
    
    // Пересечение
    Region intersection = circle1.Intersect(circle2);
    
    // Разность
    Region difference = circle1.Subtract(circle2);
}
```

### Триангуляция полигонов

```csharp
public Mesh TriangulatePolygon(Polygon polygon)
{
    // Алгоритм триангуляции
    Triangulator triangulator = new Triangulator();
    return triangulator.Triangulate(polygon);
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model2D.Geometry_Advanced_Examples.md
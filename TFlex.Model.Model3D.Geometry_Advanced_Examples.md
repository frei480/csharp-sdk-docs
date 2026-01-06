# Продвинутые примеры использования классов в пространстве имён TFlex.Model.Model3D.Geometry

## Комплексные 3D-трансформации

### Каскадные трансформации

```csharp
public AffineTransformation CreateComplexTransform()
{
    AffineTransformation transform = new AffineTransformation();
    
    // Масштабирование
    transform.Scale(2.0, 1.5, 1.0);
    
    // Вращение
    ModelAxis axis = new ModelAxis(new Point3D(0,0,0), new Direction(0,0,1));
    transform.Rotate(axis, Math.PI/4);
    
    // Перенос
    transform.Translate(10, 20, 30);
    
    return transform;
}
```

### Работа с кватернионами

```csharp
public void QuaternionOperations()
{
    Quaternion q1 = Quaternion.FromAxisAngle(new Direction(0,0,1), Math.PI/2);
    Quaternion q2 = Quaternion.FromAxisAngle(new Direction(1,0,0), Math.PI/4);
    
    // Композиция вращений
    Quaternion combined = q1 * q2;
    
    // Применение к вектору
    Direction result = combined.Rotate(new Direction(1,0,0));
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D.Geometry_Advanced_Examples.md
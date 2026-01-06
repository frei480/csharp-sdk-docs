# Примеры использования классов в пространстве имён TFlex.Model.Model3D.Visual.Manipulators

## Описание пространства имён

Пространство имён `TFlex.Model.Model3D.Visual.Manipulators` содержит классы для интерактивного манипулирования 3D-объектами.

## Основные классы

### LengthDiameterManipulator

**Пример использования:**
```csharp
LengthDiameterManipulator manipulator = new LengthDiameterManipulator();
manipulator.Length = 100.0;
manipulator.Diameter = 20.0;

// Обработка изменения значений
manipulator.ValueChanged += (sender, e) => {
    UpdateModelWithNewDimensions(manipulator.Length, manipulator.Diameter);
};
```

### RotationManipulator

**Пример вращения объектов:**
```csharp
RotationManipulator rotationManip = new RotationManipulator();
rotationManip.Axis = new Direction(0, 0, 1); // Вращение вокруг Z
rotationManip.Angle = 45.0;

// Применение вращения
rotationManip.ApplyRotation(selectedObject);
```

### ShaftManipulator

**Пример комплексного манипулятора:**
```csharp
ShaftManipulator shaftManip = new ShaftManipulator();
shaftManip.Initialize(controls, shaftData);

// Активация манипуляторов
shaftManip.Activate();

// Обработка коммита значений
shaftManip.OnValueCommitted += (sender, e) => {
    RegenerateShaftModel();
};
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D.Visual.Manipulators_Examples.md
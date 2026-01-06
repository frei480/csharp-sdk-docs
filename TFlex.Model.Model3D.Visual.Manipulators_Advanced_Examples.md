# Продвинутые примеры использования классов в пространстве имён TFlex.Model.Model3D.Visual.Manipulators

## Интерактивное манипулирование

### Комплексные манипуляторы

```csharp
public class AdvancedShaftManipulator
{
    private LengthDiameterManipulator _lengthManip;
    private RotationManipulator _rotationManip;
    private List<Manipulator> _allManipulators;
    
    public void Initialize(Document document, ShaftData shaftData)
    {
        _allManipulators = new List<Manipulator>();
        
        // Создание манипуляторов для каждого шага
        foreach (var step in shaftData.Parameters.ShaftStepList)
        {
            var lengthManip = new LengthDiameterManipulator();
            lengthManip.Length = step.Length;
            lengthManip.Diameter = step.Diameter;
            lengthManip.Position = step.Position;
            
            _allManipulators.Add(lengthManip);
        }
        
        // Глобальный манипулятор вращения
        _rotationManip = new RotationManipulator();
        _rotationManip.Axis = new Direction(0, 0, 1);
        _allManipulators.Add(_rotationManip);
    }
    
    public void Activate()
    {
        foreach (var manip in _allManipulators)
        {
            manip.Activate();
        }
    }
    
    public void Deactivate()
    {
        foreach (var manip in _allManipulators)
        {
            manip.Deactivate();
        }
    }
}
```

### Обработка событий манипуляторов

```csharp
public void SetupManipulatorEvents()
{
    _lengthManip.ValueChanged += (sender, e) => {
        var manip = sender as LengthDiameterManipulator;
        UpdateShaftDimensions(manip.Length, manip.Diameter);
        RegenerateModel();
    };
    
    _rotationManip.RotationChanged += (sender, e) => {
        var manip = sender as RotationManipulator;
        ApplyRotation(manip.Axis, manip.Angle);
    };
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D.Visual.Manipulators_Advanced_Examples.md


Руководство по T-FLEX CAD Open API

# RelativeNodeParameterX - свойство  
    
Параметр(в зависимости от значения RelationType)

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter ParameterX { get; }
```
```vb
Public ReadOnly Property ParameterX As Parameter
	Get
```
```cpp
public:
property Parameter^ ParameterX {
	Parameter^ get ();
}
```


#### Возвращаемое значение

[Parameter](T_TFlex_Model_Parameter.md)Смещение по оси X (без учёта масштаба текущей страницы) - для RelativeType.Offset. Параметр смещения - для RelativeType.OnConstruction. Параметр для определения положения узла - для RelativeType.ByParameter.

#### Ссылки

[RelativeNode - ](T_TFlex_Model_Model2D_RelativeNode.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
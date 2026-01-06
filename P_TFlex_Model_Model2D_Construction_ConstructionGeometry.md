

Руководство по T-FLEX CAD Open API

# ConstructionConstructionGeometry - свойство  
    
Геометрия линии построения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual ObjectGeometry ConstructionGeometry { get; }
```
```vb
Public Overridable ReadOnly Property ConstructionGeometry As ObjectGeometry
	Get
```
```cpp
public:
virtual property ObjectGeometry^ ConstructionGeometry {
	ObjectGeometry^ get ();
}
```


#### Значение свойства

[ObjectGeometry](T_TFlex_Model_Model2D_ObjectGeometry.md)

После использования рекомендуется удалить полученную геометрию, использую функцию Dispose().

#### Ссылки

[Construction - ](T_TFlex_Model_Model2D_Construction.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
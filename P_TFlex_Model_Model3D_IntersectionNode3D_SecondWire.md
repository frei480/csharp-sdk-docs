

Руководство по T-FLEX CAD Open API

# IntersectionNode3DSecondWire - свойство  
    
Второй элемент как проволочная модель

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Wire SecondWire { get; set; }
```
```vb
Public Property SecondWire As Wire
	Get
	Set
```
```cpp
public:
property Wire^ SecondWire {
	Wire^ get ();
	void set (Wire^ value);
}
```


#### Значение свойства

[Wire](T_TFlex_Model_Model3D_Geometry_Wire.md)

В качестве второго элемента можно задавать или проволочную модель, или ось, или солид, или листовое тело

#### Ссылки

[IntersectionNode3D - ](T_TFlex_Model_Model3D_IntersectionNode3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# IntersectionNode3DSecondSolid - свойство  
  
---  
  
Второй элемент как твёрдое тело

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Solid SecondSolid { get; set; }
```
```vb
Public Property SecondSolid As Solid
	Get
	Set
```
```cpp
public:
property Solid^ SecondSolid {
	Solid^ get ();
	void set (Solid^ value);
}
```


#### Значение свойства

[Solid](T_TFlex_Model_Model3D_Geometry_Solid.md)

В качестве второго элемента можно задавать или проволочную модель, или ось, или солид, или листовое тело

#### Ссылки

[IntersectionNode3D - ](T_TFlex_Model_Model3D_IntersectionNode3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
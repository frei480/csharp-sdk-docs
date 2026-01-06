

Руководство по T-FLEX CAD Open API

# IntersectionNode3DSecondPlane - свойство  
    
Второй элемент как листовое тело

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Workplane SecondPlane { get; set; }
```
```vb
Public Property SecondPlane As Workplane
	Get
	Set
```
```cpp
public:
property Workplane^ SecondPlane {
	Workplane^ get ();
	void set (Workplane^ value);
}
```


#### Значение свойства

[Workplane](T_TFlex_Model_Model3D_Workplane.md)

В качестве второго элемента можно задавать или проволочную модель, или ось, или солид, или листовое тело

#### Ссылки

[IntersectionNode3D - ](T_TFlex_Model_Model3D_IntersectionNode3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
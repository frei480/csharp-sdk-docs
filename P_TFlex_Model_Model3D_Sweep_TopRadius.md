

Руководство по T-FLEX CAD Open API

# SweepTopRadius - свойство  
  
---  
  
Радиус сглаживания или смещения для фаски на верхнем ребре

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter TopRadius { get; set; }
```
```vb
Public Property TopRadius As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ TopRadius {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Если значение нулевое или отрицательное, то сглаживание не строится

#### Ссылки

[Sweep - ](T_TFlex_Model_Model3D_Sweep.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
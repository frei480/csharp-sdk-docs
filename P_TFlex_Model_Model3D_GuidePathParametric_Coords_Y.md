

Руководство по T-FLEX CAD Open API

# GuidePathParametricCoordsY - свойство  
    
Переменная, в которую записывается расcчитанное значение Y-координаты точки или вектора

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Variable Y { get; set; }
```
```vb
Public Property Y As Variable
	Get
	Set
```
```cpp
public:
property Variable^ Y {
	Variable^ get ();
	void set (Variable^ value);
}
```


#### Значение свойства

[Variable](T_TFlex_Model_Variable.md)

Поскольку координата изменяется в процессе пересчета, то переменная может быть только независимой

#### Ссылки

[GuidePathParametricCoords - ](T_TFlex_Model_Model3D_GuidePathParametric_Coords.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# DirectedGuidePathParametricXSurface - свойство  
  
---  
  
Последовательность поверхностей, определяющих направление оси X

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SheetsArray XSurface { get; }
```
```vb
Public ReadOnly Property XSurface As SheetsArray
	Get
```
```cpp
public:
property SheetsArray^ XSurface {
	SheetsArray^ get ();
}
```


#### Значение свойства

[SheetsArray](T_TFlex_Model_Model3D_Geometry_SheetsArray.md)

Направление оси X задаётся одним из двух способов: путём (касательная к пути в точке) или последовательностью поверхностей (нормаль к поверхности в точке). Это обязательный параметр

#### Ссылки

[DirectedGuidePathParametric - ](T_TFlex_Model_Model3D_DirectedGuidePathParametric.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
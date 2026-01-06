

Руководство по T-FLEX CAD Open API

# OnPointsWorkplaneFaceTangentToWorkplane - свойство  
    
Поверхность, которой касается рабочая плоскость

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelFace FaceTangentToWorkplane { get; set; }
```
```vb
Public Property FaceTangentToWorkplane As ModelFace
	Get
	Set
```
```cpp
public:
property ModelFace^ FaceTangentToWorkplane {
	ModelFace^ get ();
	void set (ModelFace^ value);
}
```


#### Значение свойства

[ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)

Положение рабочей плоскости задаётся следующими способами : \- точкой и осью; \- двумя точками (возможно задание угла доворота); \- тремя точками; \- точкой и конусом или цилиндром; \- двумя точками и плоскостью (возможно задание угла доворота); \- двумя точками и направлением (возможно задание угла доворота); \- двумя точками и цилиндром, конусом или сферой;

#### Ссылки

[OnPointsWorkplane - ](T_TFlex_Model_Model3D_OnPointsWorkplane.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
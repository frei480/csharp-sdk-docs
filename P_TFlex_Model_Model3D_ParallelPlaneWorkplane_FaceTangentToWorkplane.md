

Руководство по T-FLEX CAD Open API

# ParallelPlaneWorkplaneFaceTangentToWorkplane - свойство  
    
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

Положение рабочей плоскости задаётся четырьмя взаимоисключающими способами: смещением, точкой, гранью, ребром

#### Ссылки

[ParallelPlaneWorkplane - ](T_TFlex_Model_Model3D_ParallelPlaneWorkplane.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# FaceReplaceAddFace - метод  
    
Задать пару "заменяемая грань-заменяющая поверхность"

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddFace(
	ModelFace face,
	ModelSurface surface,
	bool reverse
)
```
```vb
Public Sub AddFace ( 
	face As ModelFace,
	surface As ModelSurface,
	reverse As Boolean
)
```
```cpp
public:
void AddFace(
	ModelFace^ face, 
	ModelSurface^ surface, 
	bool reverse
)
```


#### Параметры

face [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    
surface [ModelSurface](T_TFlex_Model_Model3D_Geometry_ModelSurface.md)
    
reverse [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

surface должно быть равно 0 если задано листовое тело

#### Ссылки

[FaceReplace - ](T_TFlex_Model_Model3D_FaceReplace.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
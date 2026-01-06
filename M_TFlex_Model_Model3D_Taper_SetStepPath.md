

Руководство по T-FLEX CAD Open API

# TaperSetStepPath - метод  
    
Задать путь связанный с уклоняемой гранью

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetStepPath(
	int faceIndex,
	Path3D path
)
```
```vb
Public Sub SetStepPath ( 
	faceIndex As Integer,
	path As Path3D
)
```
```cpp
public:
void SetStepPath(
	int faceIndex, 
	Path3D^ path
)
```


#### Параметры

faceIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер уклоняемой грани
path [Path3D](T_TFlex_Model_Model3D_Path3D.md)
    Путь

Путь не может быть задан, если задано ступенчатое ребро

#### Ссылки

[Taper - ](T_TFlex_Model_Model3D_Taper.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
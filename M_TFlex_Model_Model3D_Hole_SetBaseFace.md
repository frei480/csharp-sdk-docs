

Руководство по T-FLEX CAD Open API

# HoleSetBaseFace - метод  
  
---  
  
Задать базовую грань для отверстия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool SetBaseFace(
	int hole,
	ModelFace baseFace
)
```
```vb
Public Function SetBaseFace ( 
	hole As Integer,
	baseFace As ModelFace
) As Boolean
```
```cpp
public:
bool SetBaseFace(
	int hole, 
	ModelFace^ baseFace
)
```


#### Параметры

hole [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс отверстия
baseFace [ModelFace](T_TFlex_Model_Model3D_Geometry_ModelFace.md)
    Базовая грань для отверстия

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Успешно или нет добавлена базовая грань

#### Ссылки

[Hole - ](T_TFlex_Model_Model3D_Hole.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
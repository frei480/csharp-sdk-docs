

Руководство по T-FLEX CAD Open API

# HoleSetRotation - метод  
  
---  
  
Задать поворот отверстия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool SetRotation(
	int hole,
	ModelTopol topol
)
```
```vb
Public Function SetRotation ( 
	hole As Integer,
	topol As ModelTopol
) As Boolean
```
```cpp
public:
bool SetRotation(
	int hole, 
	ModelTopol^ topol
)
```


#### Параметры

hole [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс отверстия
topol [ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)
    Элемент для поворота отверстия

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Успешно или нет добавлена базовая грань

#### Ссылки

[Hole - ](T_TFlex_Model_Model3D_Hole.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
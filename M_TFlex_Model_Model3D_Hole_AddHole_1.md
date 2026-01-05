

Руководство по T-FLEX CAD Open API

# HoleAddHole(Operation, Node3D) - метод  
  
---  
  
Добавить отверстие на грани

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool AddHole(
	Operation operation,
	Node3D node
)
```
```vb
Public Function AddHole ( 
	operation As Operation,
	node As Node3D
) As Boolean
```
```cpp
public:
bool AddHole(
	Operation^ operation, 
	Node3D^ node
)
```


#### Параметры

operation [Operation](T_TFlex_Model_Model3D_Operation.md)
    Операция, на которой строится отверстие
node [Node3D](T_TFlex_Model_Model3D_Node3D.md)
    Точка, задающая центр отверстия

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Успешно или нет добавлено отверстие

#### Ссылки

[Hole - ](T_TFlex_Model_Model3D_Hole.md)

[AddHole - перегрузка](Overload_TFlex_Model_Model3D_Hole_AddHole.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
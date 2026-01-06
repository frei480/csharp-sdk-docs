

Руководство по T-FLEX CAD Open API

# EdgeBlendingVariableBlendAttributeRemovePosition - метод  
    
Добавить позицию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void RemovePosition(
	int positionIndex
)
```
```vb
Public Sub RemovePosition ( 
	positionIndex As Integer
)
```
```cpp
public:
void RemovePosition(
	int positionIndex
)
```


#### Параметры

positionIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер позиции, должен быть в диапазоне 1..PositionCount-2

Первая и последняя позиции не могут быть удалены

#### Ссылки

[EdgeBlendingVariableBlendAttribute - ](T_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
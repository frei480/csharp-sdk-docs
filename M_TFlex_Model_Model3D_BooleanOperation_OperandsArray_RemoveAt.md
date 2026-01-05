

Руководство по T-FLEX CAD Open API

# BooleanOperationOperandsArrayRemoveAt - метод  
  
---  
  
Удалить операнд по номеру

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void RemoveAt(
	int index
)
```
```vb
Public Sub RemoveAt ( 
	index As Integer
)
```
```cpp
public:
void RemoveAt(
	int index
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер операции

Операнды нумеруются от нуля. Если индекс отрицательный или превышает количество операндов, то результат не определён

#### Ссылки

[BooleanOperationOperandsArray - ](T_TFlex_Model_Model3D_BooleanOperation_OperandsArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
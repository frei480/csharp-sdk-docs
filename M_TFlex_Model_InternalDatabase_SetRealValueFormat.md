

Руководство по T-FLEX CAD Open API

# InternalDatabaseSetRealValueFormat - метод  
    
Установить формат вещественного значения

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool SetRealValueFormat(
	int column,
	int total,
	int decimal
)
```
```vb
Public Function SetRealValueFormat ( 
	column As Integer,
	total As Integer,
	decimal As Integer
) As Boolean
```
```cpp
public:
bool SetRealValueFormat(
	int column, 
	int total, 
	int decimal
)
```


#### Параметры

column [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер столбца
total [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Общая длина
decimal [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    После запятой

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[InternalDatabase - ](T_TFlex_Model_InternalDatabase.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
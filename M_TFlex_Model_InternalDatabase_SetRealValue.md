

Руководство по T-FLEX CAD Open API

# InternalDatabaseSetRealValue - метод  
    
Установить вещественное значение в таблице

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool SetRealValue(
	int column,
	int row,
	double value
)
```
```vb
Public Function SetRealValue ( 
	column As Integer,
	row As Integer,
	value As Double
) As Boolean
```
```cpp
public:
bool SetRealValue(
	int column, 
	int row, 
	double value
)
```


#### Параметры

column [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер столбца
row [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер строки
value [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Вещественное значение

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[InternalDatabase - ](T_TFlex_Model_InternalDatabase.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
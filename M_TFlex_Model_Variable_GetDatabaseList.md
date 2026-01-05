

Руководство по T-FLEX CAD Open API

# VariableGetDatabaseList - метод  
  
---  
  
Получить параметры для формирования списка значений на основе базы данных 

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void GetDatabaseList(
	out string databaseName,
	out string fromFieldName,
	out string showFieldName,
	out string filter
)
```
```vb
Public Sub GetDatabaseList ( 
	<OutAttribute> ByRef databaseName As String,
	<OutAttribute> ByRef fromFieldName As String,
	<OutAttribute> ByRef showFieldName As String,
	<OutAttribute> ByRef filter As String
)
```
```cpp
public:
void GetDatabaseList(
	[OutAttribute] String^% databaseName, 
	[OutAttribute] String^% fromFieldName, 
	[OutAttribute] String^% showFieldName, 
	[OutAttribute] String^% filter
)
```


#### Параметры

databaseName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя базы данных
fromFieldName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя колонки базы данных, из которой будут отбираться значения
showFieldName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя колонки базы данных, которые будут появляться при отображении списка. Если колонок несколько, имена колонок в параметре разделяются точкой с запятой.
filter [String](https://learn.microsoft.com/dotnet/api/system.string)
    Условие, по которому будут отбираться значения из базы данных

#### Ссылки

[Variable - ](T_TFlex_Model_Variable.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)


Руководство по T-FLEX CAD Open API

# ListControlModelGetData - метод  
    
Возвращает данные ячейки списка

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public abstract Object GetData(
	int row,
	int column,
	ListItemRole role
)
```
```vb
Public MustOverride Function GetData ( 
	row As Integer,
	column As Integer,
	role As ListItemRole
) As Object
```
```cpp
public:
virtual Object^ GetData(
	int row, 
	int column, 
	ListItemRole role
) abstract
```


#### Параметры

row [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
column [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
role [ListItemRole](T_TFlex_Dialogs_ListItemRole.md)
    

#### Возвращаемое значение

[Object](https://learn.microsoft.com/dotnet/api/system.object)

#### Ссылки

[ListControlModel - ](T_TFlex_Dialogs_ListControlModel.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)
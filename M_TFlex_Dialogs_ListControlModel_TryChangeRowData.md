

Руководство по T-FLEX CAD Open API

# ListControlModelTryChangeRowData - метод  
  
---  
  
Попытаться изменить данные в модели.

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public virtual bool TryChangeRowData(
	int row,
	ListItemRole role,
	Object data
)
```
```vb
Public Overridable Function TryChangeRowData ( 
	row As Integer,
	role As ListItemRole,
	data As Object
) As Boolean
```
```cpp
public:
virtual bool TryChangeRowData(
	int row, 
	ListItemRole role, 
	Object^ data
)
```


#### Параметры

row [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
role [ListItemRole](T_TFlex_Dialogs_ListItemRole.md)
    
data [Object](https://learn.microsoft.com/dotnet/api/system.object)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ListControlModel - ](T_TFlex_Dialogs_ListControlModel.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)
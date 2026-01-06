

Руководство по T-FLEX CAD Open API

# ObjectSelectControlSetFilter(FuncObjectSelectControlPlainObject, Boolean, Document) - метод  
  **Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public void SetFilter(
	Func<ObjectSelectControlPlainObject, bool> canMatchDelegate,
	Document doc
)
```
```vb
Public Sub SetFilter ( 
	canMatchDelegate As Func(Of ObjectSelectControlPlainObject, Boolean),
	doc As Document
)
```
```cpp
public:
void SetFilter(
	Func<ObjectSelectControlPlainObject, bool>^ canMatchDelegate, 
	Document^ doc
)
```


#### Параметры

canMatchDelegate [Func](https://learn.microsoft.com/dotnet/api/system.func-2)[ObjectSelectControlPlainObject](T_TFlex_Dialogs_ObjectSelectControlPlainObject.md), [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
doc [Document](T_TFlex_Model_Document.md)
    

#### Ссылки

[ObjectSelectControl - ](T_TFlex_Dialogs_ObjectSelectControl.md)

[SetFilter - перегрузка](Overload_TFlex_Dialogs_ObjectSelectControl_SetFilter.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)


Руководство по T-FLEX CAD Open API

# ApplicationOpenDocumentFromDOCs(Int32, Boolean, Boolean) - метод  
  
---  
  
**Примечание: Данный API устарел.**

T-FLEX DOCs 11 больше не поддерживается

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This method is obsolete and will be removed. T-FLEX DOCs 11 no longer supported.", 
	true)]
public static Document OpenDocumentFromDOCs(
	int id,
	bool forView,
	bool visible
)
```
```vb
<ObsoleteAttribute("This method is obsolete and will be removed. T-FLEX DOCs 11 no longer supported.", 
	true)>
Public Shared Function OpenDocumentFromDOCs ( 
	id As Integer,
	forView As Boolean,
	visible As Boolean
) As Document
```
```cpp
public:
[ObsoleteAttribute(L"This method is obsolete and will be removed. T-FLEX DOCs 11 no longer supported.", 
	true)]
static Document^ OpenDocumentFromDOCs(
	int id, 
	bool forView, 
	bool visible
)
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
forView [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
visible [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)

#### Ссылки

[Application - ](T_TFlex_Application.md)

[OpenDocumentFromDOCs - перегрузка](Overload_TFlex_Application_OpenDocumentFromDOCs.md)

[TFlex - пространство имён](N_TFlex.md)


Руководство по T-FLEX CAD Open API

# DocumentDeletePage - метод  
  
---  
  
Удаление страницы

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool DeletePage(
	Page page,
	DeleteOptions options
)
```
```vb
Public Function DeletePage ( 
	page As Page,
	options As DeleteOptions
) As Boolean
```
```cpp
public:
bool DeletePage(
	Page^ page, 
	DeleteOptions^ options
)
```


#### Параметры

page [Page](T_TFlex_Model_Page.md)
    Удаляемая страница
options [DeleteOptions](T_TFlex_Model_DeleteOptions.md)
    Опции удаления

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true в случае успешного удаления, иначе false

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
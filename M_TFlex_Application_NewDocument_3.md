

Руководство по T-FLEX CAD Open API

# ApplicationNewDocument(String) - метод  
    
Создать новый документ на основе указанного файла прототипа

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Document NewDocument(
	string prototype
)
```
```vb
Public Shared Function NewDocument ( 
	prototype As String
) As Document
```
```cpp
public:
static Document^ NewDocument(
	String^ prototype
)
```


#### Параметры

prototype [String](https://learn.microsoft.com/dotnet/api/system.string)
    Путь к файлу прототипа

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Созданный документ или null в случае ошибки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[NewDocument - перегрузка](Overload_TFlex_Application_NewDocument.md)

[TFlex - пространство имён](N_TFlex.md)
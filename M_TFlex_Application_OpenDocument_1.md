

Руководство по T-FLEX CAD Open API

# ApplicationOpenDocument(String, Boolean) - метод  
  
---  
  
Открыть документ

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Document OpenDocument(
	string fileName,
	bool visible
)
```
```vb
Public Shared Function OpenDocument ( 
	fileName As String,
	visible As Boolean
) As Document
```
```cpp
public:
static Document^ OpenDocument(
	String^ fileName, 
	bool visible
)
```


#### Параметры

fileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя файла документа
visible [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает, должен ли открытый документ быть видимым

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Открытый документ или null в случае ошибки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[OpenDocument - перегрузка](Overload_TFlex_Application_OpenDocument.md)

[TFlex - пространство имён](N_TFlex.md)
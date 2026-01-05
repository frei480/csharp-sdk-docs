

Руководство по T-FLEX CAD Open API

# ApplicationOpenAsDocument(String, Boolean) - метод  
  
---  
  
Открыть документ или импортировать файл

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Document OpenAsDocument(
	string fileName,
	bool visible
)
```
```vb
Public Shared Function OpenAsDocument ( 
	fileName As String,
	visible As Boolean
) As Document
```
```cpp
public:
static Document^ OpenAsDocument(
	String^ fileName, 
	bool visible
)
```


#### Параметры

fileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя файла
visible [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает, должен ли открытый документ быть видимым

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Открытый документ или null в случае ошибки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[OpenAsDocument - перегрузка](Overload_TFlex_Application_OpenAsDocument.md)

[TFlex - пространство имён](N_TFlex.md)


Руководство по T-FLEX CAD Open API

# FileLink(Document, String, Boolean) - конструктор  
    
Конструктор ссылки на внутренний файл по пути

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public FileLink(
	Document document,
	string filePath,
	bool embedded
)
```
```vb
Public Sub New ( 
	document As Document,
	filePath As String,
	embedded As Boolean
)
```
```cpp
public:
FileLink(
	Document^ document, 
	String^ filePath, 
	bool embedded
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ ссылки
filePath [String](https://learn.microsoft.com/dotnet/api/system.string)
    Путь к ссылке
embedded [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    true, если файл вложенный

#### Ссылки

[FileLink - ](T_TFlex_Model_FileLink.md)

[FileLink - перегрузка](Overload_TFlex_Model_FileLink__ctor.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
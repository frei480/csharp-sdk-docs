

Руководство по T-FLEX CAD Open API

# ApplicationAddResourceFile(String, String) - метод  
    
Загружает строковые ресурсы из указанного файла в формате Microsoft ResX для использования в неуправляемом коде

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static bool AddResourceFile(
	string directory,
	string baseName
)
```
```vb
Public Shared Function AddResourceFile ( 
	directory As String,
	baseName As String
) As Boolean
```
```cpp
public:
static bool AddResourceFile(
	String^ directory, 
	String^ baseName
)
```


#### Параметры

directory [String](https://learn.microsoft.com/dotnet/api/system.string)
    Путь к директории, содержащей файл ресурсов, или 'null', если файл расположен в директории T-FLEX CAD
baseName [String](https://learn.microsoft.com/dotnet/api/system.string)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Данные загружаются из файла "<directory>\<baseName>.<language>.resx", где "<language>" -- двухбуквенное обозначение языка T-FLEX CAD (например, "en" для английской версии, "de" для немецкой и т.п.). Если файл с таким именем отсутствует, то часть имени файла с обозначением языка отбрасывается и попытка загрузки повторяется для файла "<directory>\<baseName>.resx".

#### Ссылки

[Application - ](T_TFlex_Application.md)

[AddResourceFile - перегрузка](Overload_TFlex_Application_AddResourceFile.md)

[TFlex - пространство имён](N_TFlex.md)


Руководство по T-FLEX CAD Open API

# StringManagerLoadResourceFile(String, String) - метод  
  
---  
  
Загружает строки из файла в формате Microsoft ResX

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool LoadResourceFile(
	string baseName,
	string path
)
```
```vb
Public Function LoadResourceFile ( 
	baseName As String,
	path As String
) As Boolean
```
```cpp
public:
bool LoadResourceFile(
	String^ baseName, 
	String^ path
)
```


#### Параметры

baseName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название файла локализации
path [String](https://learn.microsoft.com/dotnet/api/system.string)
    Путь к файлу .resx

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Загружает строки из файла "path/baseName.LC.resx" в формате Microsoft ResX. Здесь LC - двухбуквенное обозначение текущего языка. Если файл с таким именем отсутствует, будет произведена попытка загрузки с именем без обозначения кода языка. 

#### Ссылки

[StringManager - ](T_TFlex_StringManager.md)

[LoadResourceFile - перегрузка](Overload_TFlex_StringManager_LoadResourceFile.md)

[TFlex - пространство имён](N_TFlex.md)
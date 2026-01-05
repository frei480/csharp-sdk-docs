

Руководство по T-FLEX CAD Open API

# IconCreateByImagePath(String, String, Boolean) - метод  
  
---  
  
Создать объект Icon по пути к изображению

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Icon CreateByImagePath(
	string relativeFilePath,
	string rootFolderPath,
	bool cache
)
```
```vb
Public Shared Function CreateByImagePath ( 
	relativeFilePath As String,
	rootFolderPath As String,
	cache As Boolean
) As Icon
```
```cpp
public:
static Icon^ CreateByImagePath(
	String^ relativeFilePath, 
	String^ rootFolderPath, 
	bool cache
)
```


#### Параметры

relativeFilePath [String](https://learn.microsoft.com/dotnet/api/system.string)
    Относительный путь к изображению
rootFolderPath [String](https://learn.microsoft.com/dotnet/api/system.string)
    Пути к файлу изображения
cache [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Кэшировать

#### Возвращаемое значение

[Icon](T_TFlex_Dialogs_Icon.md)

#### Ссылки

[Icon - ](T_TFlex_Dialogs_Icon.md)

[CreateByImagePath - перегрузка](Overload_TFlex_Dialogs_Icon_CreateByImagePath.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)
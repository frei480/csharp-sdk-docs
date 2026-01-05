

Руководство по T-FLEX CAD Open API

# ApplicationGetSystemProfileFilePath - метод  
  
---  
  
Полный путь к системному файлу

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static string GetSystemProfileFilePath(
	string profileItemName,
	string fileName,
	bool bReadOnly
)
```
```vb
Public Shared Function GetSystemProfileFilePath ( 
	profileItemName As String,
	fileName As String,
	bReadOnly As Boolean
) As String
```
```cpp
public:
static String^ GetSystemProfileFilePath(
	String^ profileItemName, 
	String^ fileName, 
	bool bReadOnly
)
```


#### Параметры

profileItemName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя элемента окружения
fileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Document
bReadOnly [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Только на чтение. Файл не будет копироваться во временную папку, если его там еще нет.

#### Возвращаемое значение

[String](https://learn.microsoft.com/dotnet/api/system.string)

Для внутреннего использования

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)
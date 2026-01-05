

Руководство по T-FLEX CAD Open API

# ShowingImportExportDialogEventArgsAddFilter(String, Int32, String, String) - метод  
  
---  
  
Добавить фильтр к текущему диалогу

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void AddFilter(
	string filter,
	int filterID,
	string description,
	string group
)
```
```vb
Public Sub AddFilter ( 
	filter As String,
	filterID As Integer,
	description As String,
	group As String
)
```
```cpp
public:
void AddFilter(
	String^ filter, 
	int filterID, 
	String^ description, 
	String^ group
)
```


#### Параметры

filter [String](https://learn.microsoft.com/dotnet/api/system.string)
    Тип импортируемого или экспортируемого файла
filterID [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор фильтра
description [String](https://learn.microsoft.com/dotnet/api/system.string)
    Описание формата
group [String](https://learn.microsoft.com/dotnet/api/system.string)
    Группа в которую будет помещен фильтр

#### Ссылки

[ShowingImportExportDialogEventArgs - ](T_TFlex_ShowingImportExportDialogEventArgs.md)

[AddFilter - перегрузка](Overload_TFlex_ShowingImportExportDialogEventArgs_AddFilter.md)

[TFlex - пространство имён](N_TFlex.md)
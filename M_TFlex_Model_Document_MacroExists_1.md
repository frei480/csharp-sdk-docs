

Руководство по T-FLEX CAD Open API

# DocumentMacroExists(String, Boolean) - метод  
  
---  
  
Проверка наличия макроса с указанным именем

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool MacroExists(
	string macro,
	bool macroWithParameters
)
```
```vb
Public Function MacroExists ( 
	macro As String,
	macroWithParameters As Boolean
) As Boolean
```
```cpp
public:
bool MacroExists(
	String^ macro, 
	bool macroWithParameters
)
```


#### Параметры

macro [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя макроса
macroWithParameters [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Проверять макросы с аргументами

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true если макрос существует

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[MacroExists - перегрузка](Overload_TFlex_Model_Document_MacroExists.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
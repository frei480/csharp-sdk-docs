

Руководство по T-FLEX CAD Open API

# DocumentRunMacro(String, Object) - метод  
  
---  
  
Выполнить макрос с заданным именем и передать в него параметры

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Object RunMacro(
	string macro,
	params Object[] parameters
)
```
```vb
Public Function RunMacro ( 
	macro As String,
	ParamArray parameters As Object()
) As Object
```
```cpp
public:
Object^ RunMacro(
	String^ macro, 
	... array<Object^>^ parameters
)
```


#### Параметры

macro [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя макроса
parameters [Object](https://learn.microsoft.com/dotnet/api/system.object)
    Аргументы для вызова метода

#### Возвращаемое значение

[Object](https://learn.microsoft.com/dotnet/api/system.object)Возвращает результат выполнения макроса

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[RunMacro - перегрузка](Overload_TFlex_Model_Document_RunMacro.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
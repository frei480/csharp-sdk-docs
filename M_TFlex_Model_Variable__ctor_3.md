

Руководство по T-FLEX CAD Open API

# Variable(Document, String, Double, Boolean) - конструктор  
  
---  
  
Конструктор, создающий вещественную переменную с указанным значением

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Variable(
	Document document,
	string name,
	double value,
	bool external
)
```
```vb
Public Sub New ( 
	document As Document,
	name As String,
	value As Double,
	external As Boolean
)
```
```cpp
public:
Variable(
	Document^ document, 
	String^ name, 
	double value, 
	bool external
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ переменной
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя переменной
value [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Значение переменной
external [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак внешней переменной

#### Ссылки

[Variable - ](T_TFlex_Model_Variable.md)

[Variable - перегрузка](Overload_TFlex_Model_Variable__ctor.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
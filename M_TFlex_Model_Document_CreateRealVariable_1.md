

Руководство по T-FLEX CAD Open API

# DocumentCreateRealVariable(String, Double, CreateVariableMode) - метод  
    
Создает новую вещественную переменную

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Variable CreateRealVariable(
	string expression,
	ref double value,
	CreateVariableMode mode
)
```
```vb
Public Function CreateRealVariable ( 
	expression As String,
	ByRef value As Double,
	mode As CreateVariableMode
) As Variable
```
```cpp
public:
Variable^ CreateRealVariable(
	String^ expression, 
	double% value, 
	CreateVariableMode mode
)
```


#### Параметры

expression [String](https://learn.microsoft.com/dotnet/api/system.string)
    
value [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
mode [CreateVariableMode](T_TFlex_Model_CreateVariableMode.md)
    

#### Возвращаемое значение

[Variable](T_TFlex_Model_Variable.md)

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[CreateRealVariable - перегрузка](Overload_TFlex_Model_Document_CreateRealVariable.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
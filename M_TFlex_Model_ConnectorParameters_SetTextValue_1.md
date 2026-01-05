

Руководство по T-FLEX CAD Open API

# ConnectorParametersSetTextValue(String, Variable) - метод  
  
---  
  
Установить текстовое значение параметра

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int SetTextValue(
	string name,
	Variable value
)
```
```vb
Public Function SetTextValue ( 
	name As String,
	value As Variable
) As Integer
```
```cpp
public:
int SetTextValue(
	String^ name, 
	Variable^ value
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя параметра
value [Variable](T_TFlex_Model_Variable.md)
    Текстовое значение переменной

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Индекс параметра

Данный метод используется для установки выражения у параметра коннектора. Результатом выражения должно быть текстовое значение.

#### Ссылки

[ConnectorParameters - ](T_TFlex_Model_ConnectorParameters.md)

[SetTextValue - перегрузка](Overload_TFlex_Model_ConnectorParameters_SetTextValue.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
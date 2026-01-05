

Руководство по T-FLEX CAD Open API

# ConnectorParametersSetRealValue(String, Parameter) - метод  
  
---  
  
Установить вещественное значение параметра

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int SetRealValue(
	string name,
	Parameter value
)
```
```vb
Public Function SetRealValue ( 
	name As String,
	value As Parameter
) As Integer
```
```cpp
public:
int SetRealValue(
	String^ name, 
	Parameter^ value
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя параметра
value [Parameter](T_TFlex_Model_Parameter.md)
    Вещественное значение переменной

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Индекс параметра

Данный метод используется для установки выражения у параметра коннектора. Результатом выражения должно быть вещественное число.

#### Ссылки

[ConnectorParameters - ](T_TFlex_Model_ConnectorParameters.md)

[SetRealValue - перегрузка](Overload_TFlex_Model_ConnectorParameters_SetRealValue.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
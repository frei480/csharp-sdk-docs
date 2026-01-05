

Руководство по T-FLEX CAD Open API

# Parameter  \- преобразование (Variable to Parameter)  
  
---  
  
Оператор приведения к типу параметра

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static implicit operator Parameter (
	Variable var
)
```
```vb
Public Shared Widening Operator CType ( 
	var As Variable
) As Parameter
```
```cpp
static implicit operator Parameter^ (
	Variable^ var
)
```


#### Параметры

var [Variable](T_TFlex_Model_Variable.md)
    Переменная

#### Возвращаемое значение

[Parameter](T_TFlex_Model_Parameter.md)

#### Ссылки

[Parameter - ](T_TFlex_Model_Parameter.md)

[ \- перегрузка](Overload_TFlex_Model_Parameter_op_Implicit.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
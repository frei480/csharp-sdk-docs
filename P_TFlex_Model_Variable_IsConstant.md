

Руководство по T-FLEX CAD Open API

# VariableIsConstant - свойство  
    
true, если переменная является константной.

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool IsConstant { get; }
```
```vb
Public ReadOnly Property IsConstant As Boolean
	Get
```
```cpp
public:
property bool IsConstant {
	bool get ();
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Переменная является константной если её выражение состоит только из значения одного числа или текстовой константы.

#### Ссылки

[Variable - ](T_TFlex_Model_Variable.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
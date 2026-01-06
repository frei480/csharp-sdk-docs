

Руководство по T-FLEX CAD Open API

# VariableExternal - свойство  
    
true, если переменная является помеченной (внешней)

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool External { get; set; }
```
```vb
Public Property External As Boolean
	Get
	Set
```
```cpp
public:
property bool External {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Данный параметр можно установить в true только в том случае, если переменная является константной (свойство [IsConstant](P_TFlex_Model_Variable_IsConstant.md) должен возвращать true)

#### Ссылки

[Variable - ](T_TFlex_Model_Variable.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
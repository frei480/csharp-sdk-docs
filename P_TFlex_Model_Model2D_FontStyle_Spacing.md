

Руководство по T-FLEX CAD Open API

# FontStyleSpacing - свойство  
    
Дополнитальный интервал между символами

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter Spacing { get; set; }
```
```vb
Public Property Spacing As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Spacing {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Интервал между символами измеряется коэффициентом относительно размера шрифта. Стандартное значение равно 0. При значении 1 интервал между символами равен высоте шрифта.

#### Ссылки

[FontStyle - ](T_TFlex_Model_Model2D_FontStyle.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
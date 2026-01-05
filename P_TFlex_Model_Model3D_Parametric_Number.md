

Руководство по T-FLEX CAD Open API

# ParametricNumber - свойство  
  
---  
  
Переменная номера копии

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Variable Number { get; set; }
```
```vb
Public Property Number As Variable
	Get
	Set
```
```cpp
public:
property Variable^ Number {
	Variable^ get ();
	void set (Variable^ value);
}
```


#### Значение свойства

[Variable](T_TFlex_Model_Variable.md)

Значение для переменной устанавливается в процессе пересчёта от единицы до требуемого количества копий. Как правило, от переменной в номере копии зависит форма и положение исходного объекта. Поскольку номер копии изменяется в процессе пересчёта, то переменная может быть только независимой. Это обязательный параметр

#### Ссылки

[Parametric - ](T_TFlex_Model_Model3D_Parametric.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
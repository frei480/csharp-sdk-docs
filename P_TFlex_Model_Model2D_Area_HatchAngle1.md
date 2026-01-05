

Руководство по T-FLEX CAD Open API

# AreaHatchAngle1 - свойство  
  
---  
  
Первый угол штриховки контура

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter HatchAngle1 { get; set; }
```
```vb
Public Property HatchAngle1 As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ HatchAngle1 {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Данное свойство имеет смысл только в случае, если способ заполнения контура имеет значение [AreaFillStyle](T_TFlex_Model_Model2D_AreaFillStyle.md).Hatch

#### Ссылки

[Area - ](T_TFlex_Model_Model2D_Area.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
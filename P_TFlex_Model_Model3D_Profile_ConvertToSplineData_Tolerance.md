

Руководство по T-FLEX CAD Open API

# ProfileConvertToSplineDataTolerance - свойство  
  
---  
  
Точность преобразования составных контуров профиля в сплайны

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter Tolerance { get; set; }
```
```vb
Public Property Tolerance As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Tolerance {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Точность задаётся параметром, нормированным от 0.0 (грубее) до 1.0 (точнее)

#### Ссылки

[ProfileConvertToSplineData - ](T_TFlex_Model_Model3D_Profile_ConvertToSplineData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# GuidePathParametricParamFunction - свойство  
  
---  
  
Функция параметра (нормализованный параметр [0.0, 1.0])

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter ParamFunction { get; set; }
```
```vb
Public Property ParamFunction As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ ParamFunction {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Как правило, эта функция зависит от переменной номера копии. Положение начала системы координат задаётся параметром (нормализованный параметр [0.0, 1.0]) или смещением от начала пути (натуральная параметризация)

#### Ссылки

[GuidePathParametric - ](T_TFlex_Model_Model3D_GuidePathParametric.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# GuidePathParametricOffsetFunction - свойство  
    
Функция смещения от начала пути (натуральная параметризация)

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter OffsetFunction { get; set; }
```
```vb
Public Property OffsetFunction As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ OffsetFunction {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)

Как правило, эта функция зависит от переменной номера копии. Положение начала системы координат задаётся параметром (нормализованный параметр [0.0, 1.0]) или смещением от начала пути (натуральная параметризация). Один из этих переменных должна быть обязательно задана

#### Ссылки

[GuidePathParametric - ](T_TFlex_Model_Model3D_GuidePathParametric.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
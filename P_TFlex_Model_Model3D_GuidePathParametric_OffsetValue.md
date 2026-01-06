

Руководство по T-FLEX CAD Open API

# GuidePathParametricOffsetValue - свойство  
    
Переменная, в которую записывается расcчитанное значение смещения от начала пути (натуральная параметризация)

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Variable OffsetValue { get; set; }
```
```vb
Public Property OffsetValue As Variable
	Get
	Set
```
```cpp
public:
property Variable^ OffsetValue {
	Variable^ get ();
	void set (Variable^ value);
}
```


#### Значение свойства

[Variable](T_TFlex_Model_Variable.md)

Поскольку смещение изменяется в процессе пересчёта, то переменная может быть только независимой. Положение начала системы координат задаётся параметром (нормализованный параметр [ 0.0, 1.0 ]) или смещением от начала пути (натуральная параметризация). Тем не меннее, значения параметра и смещения могут также использоваться в переменных, от которых зависит форма копируемого объекта

#### Ссылки

[GuidePathParametric - ](T_TFlex_Model_Model3D_GuidePathParametric.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
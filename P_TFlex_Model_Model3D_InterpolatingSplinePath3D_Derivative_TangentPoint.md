

Руководство по T-FLEX CAD Open API

# InterpolatingSplinePath3DDerivativeTangentPoint - свойство  
    
Точка, задающая касательное условие на конце кривой

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D TangentPoint { get; set; }
```
```vb
Public Property TangentPoint As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ TangentPoint {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Касательное условие задаётся двумя взаимосиключающими методами: точкой или направлением

#### Ссылки

[InterpolatingSplinePath3DDerivative - ](T_TFlex_Model_Model3D_InterpolatingSplinePath3D_Derivative.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
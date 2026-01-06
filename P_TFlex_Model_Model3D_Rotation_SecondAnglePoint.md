

Руководство по T-FLEX CAD Open API

# RotationSecondAnglePoint - свойство  
    
Конечная точка вращения

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D SecondAnglePoint { get; set; }
```
```vb
Public Property SecondAnglePoint As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ SecondAnglePoint {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Если задаются и начальная и конечная точки вращения, то угол определяется автоматически

#### Ссылки

[Rotation - ](T_TFlex_Model_Model3D_Rotation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
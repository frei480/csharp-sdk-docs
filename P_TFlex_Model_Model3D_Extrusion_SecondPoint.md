

Руководство по T-FLEX CAD Open API

# ExtrusionSecondPoint - свойство  
    
Вторая точка, задающая направление выталкивания

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D SecondPoint { get; set; }
```
```vb
Public Property SecondPoint As ModelPoint3D
	Get
	Set
```
```cpp
public:
property ModelPoint3D^ SecondPoint {
	ModelPoint3D^ get ();
	void set (ModelPoint3D^ value);
}
```


#### Значение свойства

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)

Направление выталкивания для листовых контуров является необязательным параметром. Вектор выталкивания в явном виде задаётся направлением или двумя точками.

#### Ссылки

[Extrusion - ](T_TFlex_Model_Model3D_Extrusion.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
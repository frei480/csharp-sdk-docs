

Руководство по T-FLEX CAD Open API

# ExtrusionVector - свойство  
    
Направление выталкивания

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelDirection Vector { get; set; }
```
```vb
Public Property Vector As ModelDirection
	Get
	Set
```
```cpp
public:
property ModelDirection^ Vector {
	ModelDirection^ get ();
	void set (ModelDirection^ value);
}
```


#### Значение свойства

[ModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)

Направление выталкивания для листовых контуров является необязательным параметром. Вектор выталкивания в явном виде задаётся направлением или двумя точками

#### Ссылки

[Extrusion - ](T_TFlex_Model_Model3D_Extrusion.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
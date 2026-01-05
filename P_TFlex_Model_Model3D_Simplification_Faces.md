

Руководство по T-FLEX CAD Open API

# SimplificationFaces - свойство  
  
---  
  
Множество граней, для которых выполняется упрощение геометрии

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FacesArray Faces { get; }
```
```vb
Public ReadOnly Property Faces As FacesArray
	Get
```
```cpp
public:
property FacesArray^ Faces {
	FacesArray^ get ();
}
```


#### Значение свойства

[FacesArray](T_TFlex_Model_Model3D_FacesArray.md)

Если множество граней пусто, то упрощение геометрии выполняется на всех гранях. Все грани должны относится к одной операции, которая возвращается в свойстве Operation

#### Ссылки

[Simplification - ](T_TFlex_Model_Model3D_Simplification.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# ProfileGeometryDataToreCenter - свойство  
    
Если профиль лежит на торе, то можно получить центр тора

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelPoint3D ToreCenter { get; }
```
```vb
Public ReadOnly Property ToreCenter As ModelPoint3D
	Get
```
```cpp
public:
property ModelPoint3D^ ToreCenter {
	ModelPoint3D^ get ();
}
```


#### Возвращаемое значение

[ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md)Объект класса [ModelPoint3D](T_TFlex_Model_Model3D_Geometry_ModelPoint3D.md), хранящий координаты точки и ссылку на эти геометрические данные профиля

Для профилей, состоящих из нескольких граней или рёбер, точка может быть не определена

#### Ссылки

[ProfileGeometryData - ](T_TFlex_Model_Model3D_Profile_GeometryData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
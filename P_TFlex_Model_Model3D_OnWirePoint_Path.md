

Руководство по T-FLEX CAD Open API

# OnWirePointPath - свойство  
  
---  
  
Путь, на котором строится 3D узел

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Wire Path { get; set; }
```
```vb
Public Property Path As Wire
	Get
	Set
```
```cpp
public:
property Wire^ Path {
	Wire^ get ();
	void set (Wire^ value);
}
```


#### Значение свойства

[Wire](T_TFlex_Model_Model3D_Geometry_Wire.md)

В качестве пути можно задавать только профиль, путь, ребро. В остальных случаях узел строится не будет. При установке пути, все ранее установленные значения Offset или Param будут сброшены

#### Ссылки

[OnWirePoint - ](T_TFlex_Model_Model3D_OnWirePoint.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
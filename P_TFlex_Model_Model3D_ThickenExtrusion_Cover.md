

Руководство по T-FLEX CAD Open API

# ThickenExtrusionCover - свойство  
  
---  
  
Параметр построения крышки

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool Cover { get; set; }
```
```vb
Public Property Cover As Boolean
	Get
	Set
```
```cpp
public:
property bool Cover {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Толщина крышки должна задаваться положительным значением. Крышка строится только для плоских листовых контуров при построении стенок ненулевой длины.

#### Ссылки

[ThickenExtrusion - ](T_TFlex_Model_Model3D_ThickenExtrusion.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# CutOperationSection - свойство  
  
---  
  
Сечение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Section3D Section { get; set; }
```
```vb
Public Property Section As Section3D
	Get
	Set
```
```cpp
public:
property Section3D^ Section {
	Section3D^ get ();
	void set (Section3D^ value);
}
```


#### Значение свойства

[Section3D](T_TFlex_Model_Model3D_Section3D.md)

Поверхость сечения может задаваться тремя взаимоисключающими путями : \- набором секущих поверхностей; \- рабочей плоскостью; \- сечением. 

#### Ссылки

[CutOperation - ](T_TFlex_Model_Model3D_CutOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
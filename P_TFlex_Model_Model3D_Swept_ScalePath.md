

Руководство по T-FLEX CAD Open API

# SweptScalePath - свойство  
  
---  
  
Составной путь, задающий закон масштабирования

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public WiresArray ScalePath { get; }
```
```vb
Public ReadOnly Property ScalePath As WiresArray
	Get
```
```cpp
public:
property WiresArray^ ScalePath {
	WiresArray^ get ();
}
```


#### Значение свойства

[WiresArray](T_TFlex_Model_Model3D_Geometry_WiresArray.md)

Закон масштабирования может задаваться двумя взаимоисключающими способами : \- Составным путём; \- Табличной функцией, задающей зависимость масштаба от положения на пути в процентах.

#### Ссылки

[Swept - ](T_TFlex_Model_Model3D_Swept.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
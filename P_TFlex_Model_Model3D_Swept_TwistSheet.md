

Руководство по T-FLEX CAD Open API

# SweptTwistSheet - свойство  
    
Составной лист, задающий закон вращения

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SheetsArray TwistSheet { get; }
```
```vb
Public ReadOnly Property TwistSheet As SheetsArray
	Get
```
```cpp
public:
property SheetsArray^ TwistSheet {
	SheetsArray^ get ();
}
```


#### Значение свойства

[SheetsArray](T_TFlex_Model_Model3D_Geometry_SheetsArray.md)

Закон кручения может задаваться тремя взаимоисключающими способами : \- Составным путём; \- Табличной функцией, задающей зависимость угла кручения от положения на пути в процентах; \- Составным листом, задающим закон кручения.

#### Ссылки

[Swept - ](T_TFlex_Model_Model3D_Swept.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
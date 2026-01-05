

Руководство по T-FLEX CAD Open API

# ProfileThicknessDataGapFillType - свойство  
  
---  
  
Способы обработки разрывов

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ProfileThicknessDataGapFill GapFillType { get; set; }
```
```vb
Public Property GapFillType As ProfileThicknessDataGapFill
	Get
	Set
```
```cpp
public:
property ProfileThicknessDataGapFill GapFillType {
	ProfileThicknessDataGapFill get ();
	void set (ProfileThicknessDataGapFill value);
}
```


#### Значение свойства

[ProfileThicknessDataGapFill](T_TFlex_Model_Model3D_Profile_ThicknessData_GapFill.md)

При построении тонкостенного выталкивания для плоского контура строится эквидистантный контур. Для границ контуров, состоящих из нескольких рёбер или имеющих изломы в вершинах, возможно возникновение разрывов между эквидистантами, построенными для каждого ребра. В этом случае задаётся способ обработки такого разрыва. По умолчанию используется метод продолжения по кривой

#### Ссылки

[ProfileThicknessData - ](T_TFlex_Model_Model3D_Profile_ThicknessData.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# SweepGapFillType - свойство  
  
---  
  
Способ обработки разрывов

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SweepGapFill GapFillType { get; set; }
```
```vb
Public Property GapFillType As SweepGapFill
	Get
	Set
```
```cpp
public:
property SweepGapFill GapFillType {
	SweepGapFill get ();
	void set (SweepGapFill value);
}
```


#### Значение свойства

[SweepGapFill](T_TFlex_Model_Model3D_Sweep_GapFill.md)

При построении тонкостенного выталкивания для плоского контура строится эквидистантный контур. Для границ контуров, состоящих из нескольких рёбер или имеющих изломы в вершинах, возможно возникновение разрывов между эквидистантами, построенными для каждого ребра. В этом случае задаётся способ обработки такого разрыва. По умолчанию используется метод продолжения по кривой

#### Ссылки

[Sweep - ](T_TFlex_Model_Model3D_Sweep.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
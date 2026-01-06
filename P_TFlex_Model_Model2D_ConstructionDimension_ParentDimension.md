

Руководство по T-FLEX CAD Open API

# ConstructionDimensionParentDimension - свойство  
    
Родительский размер

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ConstructionDimension ParentDimension { set; }
```
```vb
Public WriteOnly Property ParentDimension As ConstructionDimension
	Set
```
```cpp
public:
property ConstructionDimension^ ParentDimension {
	void set (ConstructionDimension^ value);
}
```


#### Значение свойства

[ConstructionDimension](T_TFlex_Model_Model2D_ConstructionDimension.md)

В зависимости от положения родительского размера будет вычисляться значение текущего размера. Установленный родительский размер не должен иметь других родительских размеров

#### Ссылки

[ConstructionDimension - ](T_TFlex_Model_Model2D_ConstructionDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
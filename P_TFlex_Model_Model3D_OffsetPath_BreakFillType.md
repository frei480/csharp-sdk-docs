

Руководство по T-FLEX CAD Open API

# OffsetPathBreakFillType - свойство  
    
Способ обработки разрывов

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public OffsetPathBreakFill BreakFillType { get; set; }
```




#### Значение свойства

[OffsetPathBreakFill](T_TFlex_Model_Model3D_OffsetPath_BreakFill.md)

Для границ контуров, состоящих из нескольких рёбер или имеющих изломы в вершинах, возможно возникновение разрывов между эквидистантами, построенными для каждого ребра. В этом случае задаётся способ обработки такого разрыва. По умолчанию используется метод продолжения по кривой

#### Ссылки

[OffsetPath - ](T_TFlex_Model_Model3D_OffsetPath.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
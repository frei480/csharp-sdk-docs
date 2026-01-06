

Руководство по T-FLEX CAD Open API

# FaceFaceBlendGeneratorAddEdgeToBorder - метод  
    
Функция добавляет ограничительное ребро в список таких рёбер

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddEdgeToBorder(
	BaseTopol edge,
	bool invert,
	bool useCliff,
	bool invConic,
	bool сonic
)
```




#### Параметры

edge [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)
    Добавляемое ребро
invert [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак использования ребра для задания обратного касания
useCliff [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак использования ребра для задания обрезки
invConic [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак использования ребра для задания обратного конического касания
сonic [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак использования ребра для задания прямого конического касания

#### Ссылки

[FaceFaceBlendGenerator - ](T_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
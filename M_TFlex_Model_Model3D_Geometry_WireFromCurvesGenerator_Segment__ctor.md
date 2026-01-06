

Руководство по T-FLEX CAD Open API

# WireFromCurvesGeneratorSegment - конструктор  
    
Конструктор сегмента проволочного тела

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Segment(
	BaseCurve curve,
	BaseInterval interval,
	uint id
)
```




#### Параметры

curve [BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    Кривая, на которой лежит сегмент пути
interval [BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)
    Параметрический интервал кривой, на котором лежит сегмент пути
id [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Идентификатор сегмента, уникальный в границах каждого 3D объекта внешнего приложения

Использование уникальных и воспроизводимых при каждом пересчете объекта идентификаторов сегментов, позволяет обеспечить ассоциативность модели на уровне отдельных элементов топологии

#### Ссылки

[WireFromCurvesGeneratorSegment - ](T_TFlex_Model_Model3D_Geometry_WireFromCurvesGenerator_Segment.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
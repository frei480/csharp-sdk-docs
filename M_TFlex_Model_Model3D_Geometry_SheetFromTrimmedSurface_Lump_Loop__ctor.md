

Руководство по T-FLEX CAD Open API

# SheetFromTrimmedSurfaceLumpLoop - конструктор  
    
Конструктор сегмента проволочного тела

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Loop(
	BaseBody wire,
	uint id
)
```




#### Параметры

wire [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)
    Составная кривая, образующая одну из границ листового тела
id [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Идентификатор цикла, уникальный в границах каждого 3D объекта внешнего приложения

Использование уникальных и воспроизводимых при каждом пересчёте объекта идентификаторов циклов, позволяет обеспечить ассоциативность модели на уровне отдельных элементов топологии. Параметрическая область плоскость совпадает с плоскостью XY. Следовательно, составная кривая лежит в плоскости XY. Составная кривая должна быть замкнутая и не должна иметь самопересечений. Предполагается, что кривая получена в результате использования генератора WireFromCurvesGenerator

#### Ссылки

[SheetFromTrimmedSurfaceLumpLoop - ](T_TFlex_Model_Model3D_Geometry_SheetFromTrimmedSurface_Lump_Loop.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
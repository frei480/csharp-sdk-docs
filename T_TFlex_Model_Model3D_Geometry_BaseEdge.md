

Руководство по T-FLEX CAD Open API

# BaseEdge - интерфейс  
    
Базовый интерфейс для геометрических и модельных рёбер

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public interface BaseEdge
```
```vb
Public Interface BaseEdge
```
```cpp
public interface class BaseEdge
```


Тип BaseEdge предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Curve](P_TFlex_Model_Model3D_Geometry_BaseEdge_Curve.md) | Получить кривую, на которой лежит ребро |
|  | [Faces](P_TFlex_Model_Model3D_Geometry_BaseEdge_Faces.md) | Множество смежных граней |
|  | [Interval](P_TFlex_Model_Model3D_Geometry_BaseEdge_Interval.md) | Получить интервал кривой на котором лежит ребро |
|  | [Loops](P_TFlex_Model_Model3D_Geometry_BaseEdge_Loops.md) | Множество смежных циклов |
|  | [Sense](P_TFlex_Model_Model3D_Geometry_BaseEdge_Sense.md) | Получить признак совпадения ориентации кривой и ребра |
|  | [Vertices](P_TFlex_Model_Model3D_Geometry_BaseEdge_Vertices.md) | Множество вершин, смежных ребру |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [GetPolyline](M_TFlex_Model_Model3D_Geometry_BaseEdge_GetPolyline.md) | Полилиния |
|  | [GetPolyline(Double, Double, Double)](M_TFlex_Model_Model3D_Geometry_BaseEdge_GetPolyline_1.md) | Полилиния |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
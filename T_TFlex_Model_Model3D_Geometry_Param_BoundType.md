

Руководство по T-FLEX CAD Open API

# ParamBoundType - перечисление  
    
Тип ограничений значений параметра

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum BoundType
```
```vb
Public Enumeration BoundType
```
```cpp
public enum class BoundType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Infinite | 0 | Значение параметра неограничено в данном направлении |
| Extendable | 1 | Значение параметра может быть расширено в данном направлении |
| Bound | 2 | Значение параметра не может быть расширено в данном направлении |
| Closed | 3 | Концевые точки параметрического интервала совпадают |
| Degenerate | 4 | Этот параметр имеет смысл только для поверхностей. 3D геометрия для данного интервала вырожденная |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
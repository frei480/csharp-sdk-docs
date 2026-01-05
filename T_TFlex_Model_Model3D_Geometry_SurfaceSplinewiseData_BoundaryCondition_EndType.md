

Руководство по T-FLEX CAD Open API

# SurfaceSplinewiseDataBoundaryConditionEndType - перечисление  
  
---  
  
Типы условий на границах

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum EndType
```
```vb
Public Enumeration EndType
```
```cpp
public enum class EndType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Periodic | 0 | Периодический сплайн по данному направлению |
| Natural | 1 | Нулевая кривизна на границе |
| ClampedVector | 2 | Производные на границе задаются векторами |
| ClampedSpline | 3 | Производные на границе задаются сплайном (в текущей версии не поддерживается) |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
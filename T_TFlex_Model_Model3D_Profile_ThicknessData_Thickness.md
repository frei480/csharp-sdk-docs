

Руководство по T-FLEX CAD Open API

# ProfileThicknessDataThickness - перечисление  
    
Способ придания толщины

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum Thickness
```
```vb
Public Enumeration Thickness
```
```cpp
public enum class Thickness
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Outward | 0 | Стенки снаружи контура |
| Inward | 1 | Стенки изнутри контура |
| Symmetrical | 2 | Стенки симметрично наружу и внутрь |
| DoubleSided | 3 | Стенки задаются разными толщинами снаружи и изнутри |
  
Имеет смысл только для плоских контуров

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
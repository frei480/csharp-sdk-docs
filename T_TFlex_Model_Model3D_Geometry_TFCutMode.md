

Руководство по T-FLEX CAD Open API

# TFCutMode - перечисление  
    
Режимы обрезки граней при сглаживании

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum TFCutMode
```
```vb
Public Enumeration TFCutMode
```
```cpp
public enum class TFCutMode
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| bothwalls | 1 | bothwalls - обрезать по обеим стенкам |
| longwall | 2 | longwall - обрезать по длинной стенке |
| shortwall | 4 | shortwall - обрезать по короткой стенке |
| wallstrimyes | 8 | wallstrimyes - обрезать стенки и сшить всё в тело |
| wallstrimboth | 16 | wallstrimboth - обрезать стенки и не сшивать |
| wallstrimjoint | 32 | wallstrimjoint - обрезать стенки и сшить всё но твёрдое тело не образовывать |
| cutnone | 256 | cutnone - без обрезки |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
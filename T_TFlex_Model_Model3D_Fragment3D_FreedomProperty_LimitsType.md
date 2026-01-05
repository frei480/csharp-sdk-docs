

Руководство по T-FLEX CAD Open API

# Fragment3DFreedomPropertyLimitsType - перечисление  
  
---  
  
Ограничение степеней свобод

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[FlagsAttribute]
public enum LimitsType
```
```vb
<FlagsAttribute>
Public Enumeration LimitsType
```
```cpp
[FlagsAttribute]
public enum class LimitsType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| XBegin | 1 | Начало по оси X |
| XEnd | 2 | Конец по оси X |
| YBegin | 4 | Начало по оси Y |
| YEnd | 8 | Конец по оси Y |
| ZBegin | 16 | Начало по оси Z |
| ZEnd | 32 | Конец по оси Z |
| XRotation | 64 | Ограничения поворота вокруг оси X |
| YRotation | 128 | Ограничения поворота вокруг оси Y |
| ZRotation | 256 | Ограничения поворота вокруг оси Z |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
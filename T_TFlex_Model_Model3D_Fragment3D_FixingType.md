

Руководство по T-FLEX CAD Open API

# Fragment3DFixingType - перечисление  
    
Способ привязки 3D Фрагмента

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum FixingType
```
```vb
Public Enumeration FixingType
```
```cpp
public enum class FixingType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| NoFixing | 0 | Не определён |
| ByFragmentLCS | 1 | Система координат созданная в документе фрагмента в систему координат сборки |
| ByAssemblyLCS | 2 | Система координат созданная в документе сборки в систему координат сборки |
| ByWorkplane | 3 | На основе расположения 2D фрагмента на Рабочей плоскости |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
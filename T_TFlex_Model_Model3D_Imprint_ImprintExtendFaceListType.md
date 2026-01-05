

Руководство по T-FLEX CAD Open API

# ImprintImprintExtendFaceListType - перечисление  
  
---  
  
Варианты расширения списка обрабатываемых граней при построении пересечений. Определяют способ выбора соседних граней

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum ImprintExtendFaceListType
```
```vb
Public Enumeration ImprintExtendFaceListType
```
```cpp
public enum class ImprintExtendFaceListType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| No | 0 | Не выбирать |
| Target | 1 | Выбирать только разделяемые |
| Tool | 2 | Выбирать только разделяющие |
| All | 3 | Выбирать разделяемые и разделяющие |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
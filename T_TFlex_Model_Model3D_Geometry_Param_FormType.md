

Руководство по T-FLEX CAD Open API

# ParamFormType - перечисление  
    
Отношение между параметризацией и пространственной величиной

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum FormType
```
```vb
Public Enumeration FormType
```
```cpp
public enum class FormType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Linear | 0 | Параметр пропорционален расстоянию вдоль прямой. Для поверхности прямой линии соответствует изолиния по другому параметру |
| Circular | 1 | Параметр является углом окружности. Для поверхности окружность соответствует изолиния по другому параметру |
| Any | 2 | Все остальные случаи |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
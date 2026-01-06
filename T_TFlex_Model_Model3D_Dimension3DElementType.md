

Руководство по T-FLEX CAD Open API

# Dimension3DElementType - перечисление  
    
Типы объектов для 3D размеров

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum Dimension3DElementType
```
```vb
Public Enumeration Dimension3DElementType
```
```cpp
public enum class Dimension3DElementType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Wrong | 0 | Тип не совпадает с объектом |
| Plane | 1 | Плоскость (для плоских граней и плоских ребер) |
| Axis | 2 | Ось (для ребер, циллиндрических граней, ребер-окружностей) |
| Point | 3 | Точка (для узлов) |
| Circle | 4 | Окружность (для циллиндрических, сферических и тороидальных граней, ребер-окружностей) |
| AxisX | 5 | Ось X (для ЛСК) |
| AxisY | 6 | Ось Y (для ЛСК) |
| AxisZ | 7 | Ось Z (для ЛСК) |
| Undefined | -1 | Не задан |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
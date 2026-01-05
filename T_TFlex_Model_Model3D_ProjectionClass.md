

Руководство по T-FLEX CAD Open API

# ProjectionClass - перечисление  
  
---  
  
Типы проекций с невидимыми линиями

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public enum ProjectionClass
```
```vb
Public Enumeration ProjectionClass
```
```cpp
public enum class ProjectionClass
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| HiddenRemoved | 0 | Вид с удалёнными невидимыми линиями |
| AllVisible | 1 | Вид без удаления невидимых линий |
| ShadedImage | 2 | Тоновая закраска без материалов |
| RenderImage | 3 | Тоновая закраска c материалами |
| QuickHidden | 4 | Удаление невидимых линий с использованием растрового алгоритма |
| DrawEdge | 5 | Рисовать рёбра при работе с растровыми проекциями |
| DrawOutlines | 6 | Рисовать очерки при работе с растровыми проекциями |
| VectorImage | 7 | Векторная картинка |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
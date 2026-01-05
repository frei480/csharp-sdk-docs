

Руководство по T-FLEX CAD Open API

# OutlineType - перечисление  
  
---  
  
Подтипы линий изображения

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum OutlineType
```
```vb
Public Enumeration OutlineType
```
```cpp
public enum class OutlineType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Undefined | 0 | Не определён |
| ConstructionOutline | 1 | Линия изображения, основанная на узлах и линиях построения. Класс [ConstructionOutline](T_TFlex_Model_Model2D_ConstructionOutline.md) |
| CopyOutline | 2 | Линия изображения, полученная ассоциативным копированием. Класс [CopyOutline](T_TFlex_Model_Model2D_CopyOutline.md) |
| ProjectionOutline | 3 | Линия изображения, принадлежащая 2D проекции. Класс [ProjectionOutline](T_TFlex_Model_Model3D_ProjectionOutline.md) |
| FragmentOutline | 4 | Линия изображения, поднятая с фрагмента. Класс [FragmentOutline](T_TFlex_Model_Model2D_FragmentOutline.md) |
| CircleOutline | 5 | Линия изображения - окружность с центром в узле с заданным радиусом. Класс [CircleOutline](T_TFlex_Model_Model2D_CircleOutline.md) |
| ThreePointArcOutline | 6 | Линия изображения - дуга окружности, проходящая через три узла. Класс [ThreePointArcOutline](T_TFlex_Model_Model2D_ThreePointArcOutline.md) |
| TwoPointArcOutline | 7 | Линия изображения - дуга окружности, проходящая через два узла с заданным радиусом. Класс [TwoPointArcOutline](T_TFlex_Model_Model2D_TwoPointArcOutline.md) |
| TwoPointCircleOutline | 8 | Линия изображения - окружность, проходящая через два узла с заданным радиусом. Класс [TwoPointCircleOutline](T_TFlex_Model_Model2D_TwoPointCircleOutline.md) |
| CenterAxisOutline | 9 | Линия изображения - ось окружности или эллипса. Класс [CenterAxisOutline](T_TFlex_Model_Model2D_CenterAxisOutline.md) |
| AxisOutline | 10 | Линия изображения - ось двух других линий изображения. Класс [AxisOutline](T_TFlex_Model_Model2D_AxisOutline.md) |
| PolylineOutline | 11 |  |
| CircleToCircleAxisOutline | 12 | Линия изображения - ось между двумя окружностями. Класс [CircleToCircleAxisOutline](T_TFlex_Model_Model2D_CircleToCircleAxisOutline.md) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
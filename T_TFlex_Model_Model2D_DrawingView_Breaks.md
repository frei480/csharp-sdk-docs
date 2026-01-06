

Руководство по T-FLEX CAD Open API

# DrawingViewBreaks - класс  
    
Набор разрывов чертёжного вида

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model2DDrawingViewBreaks

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class Breaks : IEnumerable<DrawingViewBreak>
```




Тип DrawingViewBreaks предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Alignment](P_TFlex_Model_Model2D_DrawingView_Breaks_Alignment.md) | **Устарело.** Способ задания позиций разрывов чертёжного вида, в соответствии с направлением разрывов(по вертикали) |
|  | [Angle](P_TFlex_Model_Model2D_DrawingView_Breaks_Angle.md) | Угол направления разрывов |
|  | [AngleLine](P_TFlex_Model_Model2D_DrawingView_Breaks_AngleLine.md) | Прямая, задающая направление разрывов (допускается значение null) |
|  | [BrokenBoundConstruction1](P_TFlex_Model_Model2D_DrawingView_Breaks_BrokenBoundConstruction1.md) | Первая линия построения, задающая границу для линий разрывов (допускается значение null) |
|  | [BrokenBoundConstruction2](P_TFlex_Model_Model2D_DrawingView_Breaks_BrokenBoundConstruction2.md) | Вторая линия построения, задающая границу для линий разрывов (допускается значение null) |
|  | [BrokenBoundOutline1](P_TFlex_Model_Model2D_DrawingView_Breaks_BrokenBoundOutline1.md) | Первая линия изображения, задающая границу для линий разрывов (допускается значение null) |
|  | [BrokenBoundOutline2](P_TFlex_Model_Model2D_DrawingView_Breaks_BrokenBoundOutline2.md) | Вторая линия изображения, задающая границу для линий разрывов (допускается значение null) |
|  | [Count](P_TFlex_Model_Model2D_DrawingView_Breaks_Count.md) | Количество разрывов |
|  | [Gap](P_TFlex_Model_Model2D_DrawingView_Breaks_Gap.md) | Размер разрыва в единицах страницы |
|  | [HorizontalAlignment](P_TFlex_Model_Model2D_DrawingView_Breaks_HorizontalAlignment.md) | Способ задания позиций разрывов чертёжного вида, в соответствии с направлением разрывов(по горизонтали) |
|  | [Item](P_TFlex_Model_Model2D_DrawingView_Breaks_Item.md) |  |
|  | [KeepParts](P_TFlex_Model_Model2D_DrawingView_Breaks_KeepParts.md) | Сохранять части изображения в исходном положении |
|  | [LineColor](P_TFlex_Model_Model2D_DrawingView_Breaks_LineColor.md) | Цвет линий разрыва |
|  | [LineExtension](P_TFlex_Model_Model2D_DrawingView_Breaks_LineExtension.md) | Размер выступания линий разрыва в единицах страницы |
|  | [LineScale](P_TFlex_Model_Model2D_DrawingView_Breaks_LineScale.md) | Масштаб штрихов линий разрыва |
|  | [LineType](P_TFlex_Model_Model2D_DrawingView_Breaks_LineType.md) | Тип линий разрыва |
|  | [LineWaveHeight](P_TFlex_Model_Model2D_DrawingView_Breaks_LineWaveHeight.md) | Высота волны волнистой линии |
|  | [LineWaveLength](P_TFlex_Model_Model2D_DrawingView_Breaks_LineWaveLength.md) | Длина периода волнистой линии |
|  | [LineWaveNumber](P_TFlex_Model_Model2D_DrawingView_Breaks_LineWaveNumber.md) | Количество периодов волнистой линии |
|  | [LineWaveType](P_TFlex_Model_Model2D_DrawingView_Breaks_LineWaveType.md) | Способ задания волнистой линии |
|  | [LineWidth](P_TFlex_Model_Model2D_DrawingView_Breaks_LineWidth.md) | Толщина линий разрыва |
|  | [Metric](P_TFlex_Model_Model2D_DrawingView_Breaks_Metric.md) | Способ задания позиций разрывов чертёжного вида |
|  | [Origin](P_TFlex_Model_Model2D_DrawingView_Breaks_Origin.md) | Базовая точка разрывов |
|  | [OriginNode](P_TFlex_Model_Model2D_DrawingView_Breaks_OriginNode.md) | Базовый узел разрывов (допускается значение null) |
|  | [SpecialElements](P_TFlex_Model_Model2D_DrawingView_Breaks_SpecialElements.md) | Получить коллекцию элементов, управляющих отображением 2D объектов в области разрыва на чертёжном виде |
|  | [UseLineColor](P_TFlex_Model_Model2D_DrawingView_Breaks_UseLineColor.md) | Использовать особый цвет линий разрыва |
|  | [UseLineExtension](P_TFlex_Model_Model2D_DrawingView_Breaks_UseLineExtension.md) | Показывать линии разрыва с выступами |
|  | [VerticalAlignment](P_TFlex_Model_Model2D_DrawingView_Breaks_VerticalAlignment.md) | Способ задания позиций разрывов чертёжного вида, в соответствии с направлением разрывов(по вертикали) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddBreak](M_TFlex_Model_Model2D_DrawingView_Breaks_AddBreak.md) | Добавить разрыв |
|  | [AddBreak(Boolean)](M_TFlex_Model_Model2D_DrawingView_Breaks_AddBreak_1.md) | Добавить разрыв |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAt](M_TFlex_Model_Model2D_DrawingView_Breaks_GetAt.md) | Получить разрыв по индексу |
|  | [GetEnumerator](M_TFlex_Model_Model2D_DrawingView_Breaks_GetEnumerator.md) | Получить перечиcлитель |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAll](M_TFlex_Model_Model2D_DrawingView_Breaks_RemoveAll.md) | Удалить все разрывы |
|  | [RemoveAt](M_TFlex_Model_Model2D_DrawingView_Breaks_RemoveAt.md) | Добавить разрыв |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Update](M_TFlex_Model_Model2D_DrawingView_Breaks_Update.md) | Обновление габаритов разрывов чертежного вида |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
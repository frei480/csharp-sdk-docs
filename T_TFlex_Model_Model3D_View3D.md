

Руководство по T-FLEX CAD Open API

# View3D - класс  
    
Данный класс представляет собой 3D вид документа

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelView](T_TFlex_Model_View.md) TFlex.Model.Model3DView3D

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class View3D : View
```
```vb
Public NotInheritable Class View3D
	Inherits View
```
```cpp
public ref class View3D sealed : public View
```


Тип View3D предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [CurrentObject](P_TFlex_Model_Model3D_View3D_CurrentObject.md) | Объект, выбранный под мышкой |
|  | [DecorationScale](P_TFlex_Model_Model3D_View3D_DecorationScale.md) | Возвращает коэффициент, используемый для определения шага манипуляторов |
|  | [Document](P_TFlex_Model_View_Document.md) | Документ, видом которого является данный объект(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Frustum](P_TFlex_Model_Model3D_View3D_Frustum.md) |  |
|  | [Graphics](P_TFlex_Model_View_Graphics.md) | Объект графического контекста для вывода графического изображения в данный вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [HideConstructions](P_TFlex_Model_View_HideConstructions.md) | Параметр "Скрыть линии построения"(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [HWnd](P_TFlex_Model_View_HWnd.md) | Дескриптор окна вида(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Orientation](P_TFlex_Model_Model3D_View3D_Orientation.md) |  |
|  | [Page](P_TFlex_Model_View_Page.md) | Страница, которая отображается в данном виде(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [RecommendedDraggerStep](P_TFlex_Model_Model3D_View3D_RecommendedDraggerStep.md) | Возвращает рекомендованное значение шага манипулятора при текущем приближении |
|  | [Scene](P_TFlex_Model_Model3D_View3D_Scene.md) | Сцена, изображаемая в этом виде |
|  | [Translation](P_TFlex_Model_Model3D_View3D_Translation.md) |  |
|  | [TreeViewRect](P_TFlex_Model_Model3D_View3D_TreeViewRect.md) | Положение окна дерева модели |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Model_View_Activate.md) | Активизировать вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [ActivateWorkplane](M_TFlex_Model_Model3D_View3D_ActivateWorkplane.md) | Переводит окно в режим черчения на рабочей плоскости. |
|  | [ApplyTranform](M_TFlex_Model_Model3D_View3D_ApplyTranform.md) |  |
|  | [Close](M_TFlex_Model_View_Close.md) | Закрыть вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [DeactivateWorkplane](M_TFlex_Model_Model3D_View3D_DeactivateWorkplane.md) | Завершает режим черчения на рабочей плоскости. |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindBoundBox](M_TFlex_Model_Model3D_View3D_FindBoundBox.md) | Получить границы 3D сцены |
|  | [GetDefaultParameters](M_TFlex_Model_Model3D_View3D_GetDefaultParameters.md) | Получить параметры 3D вида по умолчанию для новых видов |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetParameters](M_TFlex_Model_Model3D_View3D_GetParameters.md) | Получить параметры 3D вида |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Insert3DFragment](M_TFlex_Model_Model3D_View3D_Insert3DFragment.md) |  |
|  | [InsertRender](M_TFlex_Model_Model3D_View3D_InsertRender.md) |  |
|  | [MoveCameraToContainPoints](M_TFlex_Model_Model3D_View3D_MoveCameraToContainPoints.md) |  |
|  | [Pick](M_TFlex_Model_Model3D_View3D_Pick.md) | Ищет точку на декорации по заданным экранным координатам |
|  | [PointToClient](M_TFlex_Model_View_PointToClient.md) | Преобразование точки из экранных координат в оконные(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [PointToModel](M_TFlex_Model_View_PointToModel.md) | Преобразование точки из экранных координат в модельные(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [PointToRay](M_TFlex_Model_Model3D_View3D_PointToRay.md) | Преобразует точку на экране в луч в координатах модели |
|  | [PointToScreen](M_TFlex_Model_View_PointToScreen.md) | Преобразование точки из оконных координат в экранные(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [RemoveRender](M_TFlex_Model_Model3D_View3D_RemoveRender.md) |  |
|  | [Search(Point, SelectionFilter, Double)](M_TFlex_Model_View_Search_1.md) | Поиск элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Search(Double, Double, SelectionFilter, Double)](M_TFlex_Model_View_Search.md) | Поиск элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Point, SelectionFilter)](M_TFlex_Model_View_Select_1.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Int32, Int32, SelectionFilter)](M_TFlex_Model_View_Select_2.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Point, SelectionFilter, Double)](M_TFlex_Model_View_Select_3.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Double, Double, SelectionFilter, Double)](M_TFlex_Model_View_Select.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [SetCursor](M_TFlex_Model_View_SetCursor.md) | Установить курсор(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [SetDefaultParameters](M_TFlex_Model_Model3D_View3D_SetDefaultParameters.md) | Установить параметры 3D вида по умолчанию для новых видов |
|  | [SetParameters](M_TFlex_Model_Model3D_View3D_SetParameters.md) | Установить параметры 3D вида |
|  | [ShowObject](M_TFlex_Model_Model3D_View3D_ShowObject.md) | Изменить масштаб изображения, чтобы показать объект |
|  | [Split](M_TFlex_Model_View_Split.md) | Разделить вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [SplitHorizontally](M_TFlex_Model_View_SplitHorizontally.md) | Разделить по горизонтали(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [SplitVertically](M_TFlex_Model_View_SplitVertically.md) | Разделить по вертикали(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UpdateBoundBox](M_TFlex_Model_Model3D_View3D_UpdateBoundBox.md) |  |
|  | [Zoom](M_TFlex_Model_Model3D_View3D_Zoom.md) | Увеличить или уменьшить изображение |
|  | [ZoomAll](M_TFlex_Model_Model3D_View3D_ZoomAll.md) | Показать все объекты |
|  | [ZoomIn](M_TFlex_Model_Model3D_View3D_ZoomIn.md) | Увеличить изображение |
|  | [ZoomOut](M_TFlex_Model_Model3D_View3D_ZoomOut.md) | Уменьшить изображение |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# View2D - класс  
  
---  
  
Данный класс представляет собой 2D вид документа.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelView](T_TFlex_Model_View.md) TFlex.Model.Model2DView2D

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class View2D : View
```
```vb
Public NotInheritable Class View2D
	Inherits View
```
```cpp
public ref class View2D sealed : public View
```


Тип View2D предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [BasePage](P_TFlex_Model_Model2D_View2D_BasePage.md) | Страница, которая отображается в данном виде, без учёта активированных DrawingView |
|  | [Document](P_TFlex_Model_View_Document.md) | Документ, видом которого является данный объект(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Graphics](P_TFlex_Model_View_Graphics.md) | Объект графического контекста для вывода графического изображения в данный вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [HasActivatedDrawingViews](P_TFlex_Model_Model2D_View2D_HasActivatedDrawingViews.md) | Есть ли активированный чертёжный вид хотя бы на одной странице вида |
|  | [HideConstructions](P_TFlex_Model_View_HideConstructions.md) | Параметр "Скрыть линии построения"(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [HWnd](P_TFlex_Model_View_HWnd.md) | Дескриптор окна вида(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Page](P_TFlex_Model_View_Page.md) | Страница, которая отображается в данном виде(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [ZoomRectangle](P_TFlex_Model_Model2D_View2D_ZoomRectangle.md) | Прямоугольник, который отображается в данном виде |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Model_View_Activate.md) | Активизировать вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Close](M_TFlex_Model_View_Close.md) | Закрыть вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [PointToClient](M_TFlex_Model_View_PointToClient.md) | Преобразование точки из экранных координат в оконные(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [PointToModel](M_TFlex_Model_View_PointToModel.md) | Преобразование точки из экранных координат в модельные(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [PointToScreen](M_TFlex_Model_View_PointToScreen.md) | Преобразование точки из оконных координат в экранные(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Search(Point, SelectionFilter, Double)](M_TFlex_Model_View_Search_1.md) | Поиск элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Search(Double, Double, SelectionFilter, Double)](M_TFlex_Model_View_Search.md) | Поиск элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Point, SelectionFilter)](M_TFlex_Model_View_Select_1.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Int32, Int32, SelectionFilter)](M_TFlex_Model_View_Select_2.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Point, SelectionFilter, Double)](M_TFlex_Model_View_Select_3.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Select(Double, Double, SelectionFilter, Double)](M_TFlex_Model_View_Select.md) | Выбор элемента модели(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [SetCursor](M_TFlex_Model_View_SetCursor.md) | Установить курсор(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [Split](M_TFlex_Model_View_Split.md) | Разделить вид(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [SplitHorizontally](M_TFlex_Model_View_SplitHorizontally.md) | Разделить по горизонтали(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [SplitVertically](M_TFlex_Model_View_SplitVertically.md) | Разделить по вертикали(Унаследован от [View](T_TFlex_Model_View.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
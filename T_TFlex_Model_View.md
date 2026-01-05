

Руководство по T-FLEX CAD Open API

# View - класс  
  
---  
  
Данный класс реализует функциональность вида документа

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelView [TFlex.Model.Model2DView2D](T_TFlex_Model_Model2D_View2D.md) [TFlex.Model.Model3DView3D](T_TFlex_Model_Model3D_View3D.md)

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class View
```
```vb
Public MustInherit Class View
```
```cpp
public ref class View abstract
```


Тип View предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Document](P_TFlex_Model_View_Document.md) | Документ, видом которого является данный объект |
|  | [Graphics](P_TFlex_Model_View_Graphics.md) | Объект графического контекста для вывода графического изображения в данный вид |
|  | [HideConstructions](P_TFlex_Model_View_HideConstructions.md) | Параметр "Скрыть линии построения" |
|  | [HWnd](P_TFlex_Model_View_HWnd.md) | Дескриптор окна вида |
|  | [Page](P_TFlex_Model_View_Page.md) | Страница, которая отображается в данном виде |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Model_View_Activate.md) | Активизировать вид |
|  | [Close](M_TFlex_Model_View_Close.md) | Закрыть вид |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [PointToClient](M_TFlex_Model_View_PointToClient.md) | Преобразование точки из экранных координат в оконные |
|  | [PointToModel](M_TFlex_Model_View_PointToModel.md) | Преобразование точки из экранных координат в модельные |
|  | [PointToScreen](M_TFlex_Model_View_PointToScreen.md) | Преобразование точки из оконных координат в экранные |
|  | [Search(Point, SelectionFilter, Double)](M_TFlex_Model_View_Search_1.md) | Поиск элемента модели |
|  | [Search(Double, Double, SelectionFilter, Double)](M_TFlex_Model_View_Search.md) | Поиск элемента модели |
|  | [Select(Point, SelectionFilter)](M_TFlex_Model_View_Select_1.md) | Выбор элемента модели |
|  | [Select(Int32, Int32, SelectionFilter)](M_TFlex_Model_View_Select_2.md) | Выбор элемента модели |
|  | [Select(Point, SelectionFilter, Double)](M_TFlex_Model_View_Select_3.md) | Выбор элемента модели |
|  | [Select(Double, Double, SelectionFilter, Double)](M_TFlex_Model_View_Select.md) | Выбор элемента модели |
|  | [SetCursor](M_TFlex_Model_View_SetCursor.md) | Установить курсор |
|  | [Split](M_TFlex_Model_View_Split.md) | Разделить вид |
|  | [SplitHorizontally](M_TFlex_Model_View_SplitHorizontally.md) | Разделить по горизонтали |
|  | [SplitVertically](M_TFlex_Model_View_SplitVertically.md) | Разделить по вертикали |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Класс является базовым классом для классов [View2D](T_TFlex_Model_Model2D_View2D.md) и [View3D](T_TFlex_Model_Model3D_View3D.md), являющимися 2D и 3D видами соответственно

#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
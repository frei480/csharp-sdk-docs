

Руководство по T-FLEX CAD Open API

# LineDragger - класс  
    
**Примечание: Данный API устарел.**

Манипулятор для линейного изменения данных

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.VisualDragger](T_TFlex_Model_Model3D_Visual_Dragger.md) TFlex.Model.Model3D.VisualLineDragger

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")]
public class LineDragger : Dragger
```
```vb
<ObsoleteAttribute("This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")>
Public Class LineDragger
	Inherits Dragger
```
```cpp
[ObsoleteAttribute(L"This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")]
public ref class LineDragger : public Dragger
```


Тип LineDragger предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [LineDragger](M_TFlex_Model_Model3D_Visual_LineDragger__ctor.md) | Конструктор по умолчанию |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Addition](P_TFlex_Model_Model3D_Visual_Dragger_Addition.md) | Дополнительная информация(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Cursor](P_TFlex_Model_Model3D_Visual_Dragger_Cursor.md) | Курсор(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Decoration](P_TFlex_Model_Model3D_Visual_Dragger_Decoration.md) | Связанная декорация(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Direction](P_TFlex_Model_Model3D_Visual_LineDragger_Direction.md) | Направление, вдоль которого измеряется перемещение |
|  | [FromOrigin](P_TFlex_Model_Model3D_Visual_LineDragger_FromOrigin.md) | Значение драггера считается от начальной точки или от точки клика |
|  | [MaximalValue](P_TFlex_Model_Model3D_Visual_Dragger_MaximalValue.md) | Максимальное значение(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [MaximalValueEnabled](P_TFlex_Model_Model3D_Visual_Dragger_MaximalValueEnabled.md) | Использование максимального значения(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [MinimalValue](P_TFlex_Model_Model3D_Visual_Dragger_MinimalValue.md) | Минимальное значение(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [MinimalValueEnabled](P_TFlex_Model_Model3D_Visual_Dragger_MinimalValueEnabled.md) | Использование минимального значения(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Origin](P_TFlex_Model_Model3D_Visual_LineDragger_Origin.md) | Начальная точка, от которой измеряется перемещение |
|  | [Step](P_TFlex_Model_Model3D_Visual_LineDragger_Step.md) | (Переопределяет [DraggerStep](P_TFlex_Model_Model3D_Visual_Dragger_Step.md)) |
|  | [Transparent](P_TFlex_Model_Model3D_Visual_Dragger_Transparent.md) | Возможность выбора объектов, скрытых манипулятором(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Value](P_TFlex_Model_Model3D_Visual_LineDragger_Value.md) | Текущее значение(Переопределяет [DraggerValue](P_TFlex_Model_Model3D_Visual_Dragger_Value.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Model_Model3D_Visual_LineDragger_Activate.md) | Переопределённый метод класса Dragger(Переопределяет [DraggerActivate(View3D, Int32, Int32, Single)](M_TFlex_Model_Model3D_Visual_Dragger_Activate.md)) |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Dragger_Dispose.md) | (Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_Dragger_Dispose_1.md) | (Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindClosestPoint](M_TFlex_Model_Model3D_Visual_Dragger_FindClosestPoint.md) | Поиск ближайшей точки на декорациях(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Release](M_TFlex_Model_Model3D_Visual_LineDragger_Release.md) | Переопределённый метод класса Dragger(Переопределяет [DraggerRelease](M_TFlex_Model_Model3D_Visual_Dragger_Release.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UpdatePosition](M_TFlex_Model_Model3D_Visual_LineDragger_UpdatePosition.md) | Переопределённый метод класса Dragger(Переопределяет [DraggerUpdatePosition(View3D, Int32, Int32)](M_TFlex_Model_Model3D_Visual_Dragger_UpdatePosition.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activated](E_TFlex_Model_Model3D_Visual_Dragger_Activated.md) | Событие происходит после того, как метод Activated возвращает true(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Released](E_TFlex_Model_Model3D_Visual_Dragger_Released.md) | Событие происходит после выхода из метода Release(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
|  | [Updated](E_TFlex_Model_Model3D_Visual_Dragger_Updated.md) | Событие происходит после того, как метод UpdatePosition возвращает true(Унаследован от [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)) |
  
Манипулятор позволяет изменять данные с помощью перемещения декораций вдоль заданной оси. 

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)

[DraggerManager](T_TFlex_Model_Model3D_Visual_DraggerManager.md)

[Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)

[CircleDragger](T_TFlex_Model_Model3D_Visual_CircleDragger.md)

[DraggerManager](T_TFlex_Model_Model3D_Visual_DraggerManager.md)

[Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)

[CircleDragger](T_TFlex_Model_Model3D_Visual_CircleDragger.md)
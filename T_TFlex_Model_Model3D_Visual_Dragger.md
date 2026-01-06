

Руководство по T-FLEX CAD Open API

# Dragger - класс  
    
**Примечание: Данный API устарел.**

Манипулятор

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.VisualDragger [TFlex.Model.Model3D.VisualCircleDragger](T_TFlex_Model_Model3D_Visual_CircleDragger.md) [TFlex.Model.Model3D.VisualLineDragger](T_TFlex_Model_Model3D_Visual_LineDragger.md) [TFlex.Model.Model3D.VisualRadiusDragger](T_TFlex_Model_Model3D_Visual_RadiusDragger.md)

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")]
public abstract class Dragger : IDisposable
```
```vb
<ObsoleteAttribute("This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")>
Public MustInherit Class Dragger
	Implements IDisposable
```
```cpp
[ObsoleteAttribute(L"This class is obsolete and will be removed. Please use 'Manipulator' class and types from 'Manipulators' namespace.")]
public ref class Dragger abstract : IDisposable
```


#### Значение поля

Базовый класс для всех манипуляторов. В порождённом классе необходимо перекрыть методы Activate и UpdatePosition, при необходимости и Release. После создания манипулятора нужно связать его с [Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md), декорацией и зарегистрировать в [DraggerManager](T_TFlex_Model_Model3D_Visual_DraggerManager.md), диспетчере. 

Тип Dragger предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Dragger](M_TFlex_Model_Model3D_Visual_Dragger__ctor.md) | Конструктор по умолчанию |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Addition](P_TFlex_Model_Model3D_Visual_Dragger_Addition.md) | Дополнительная информация |
|  | [Cursor](P_TFlex_Model_Model3D_Visual_Dragger_Cursor.md) | Курсор |
|  | [Decoration](P_TFlex_Model_Model3D_Visual_Dragger_Decoration.md) | Связанная декорация |
|  | [MaximalValue](P_TFlex_Model_Model3D_Visual_Dragger_MaximalValue.md) | Максимальное значение |
|  | [MaximalValueEnabled](P_TFlex_Model_Model3D_Visual_Dragger_MaximalValueEnabled.md) | Использование максимального значения |
|  | [MinimalValue](P_TFlex_Model_Model3D_Visual_Dragger_MinimalValue.md) | Минимальное значение |
|  | [MinimalValueEnabled](P_TFlex_Model_Model3D_Visual_Dragger_MinimalValueEnabled.md) | Использование минимального значения |
|  | [Step](P_TFlex_Model_Model3D_Visual_Dragger_Step.md) | Текущий шаг |
|  | [Transparent](P_TFlex_Model_Model3D_Visual_Dragger_Transparent.md) | Возможность выбора объектов, скрытых манипулятором |
|  | [Value](P_TFlex_Model_Model3D_Visual_Dragger_Value.md) | Текущее значение |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activate](M_TFlex_Model_Model3D_Visual_Dragger_Activate.md) | Активизация манипулятора |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Dragger_Dispose.md) | Освобождает все ресурсы, используемые объектом Dragger |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_Dragger_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом Dragger, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FindClosestPoint](M_TFlex_Model_Model3D_Visual_Dragger_FindClosestPoint.md) | Поиск ближайшей точки на декорациях |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Release](M_TFlex_Model_Model3D_Visual_Dragger_Release.md) | Конец перемещения |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [UpdatePosition](M_TFlex_Model_Model3D_Visual_Dragger_UpdatePosition.md) | Обновление положения |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Activated](E_TFlex_Model_Model3D_Visual_Dragger_Activated.md) | Событие происходит после того, как метод Activated возвращает true |
|  | [Released](E_TFlex_Model_Model3D_Visual_Dragger_Released.md) | Событие происходит после выхода из метода Release |
|  | [Updated](E_TFlex_Model_Model3D_Visual_Dragger_Updated.md) | Событие происходит после того, как метод UpdatePosition возвращает true |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(Dragger, Dragger)](M_TFlex_Model_Model3D_Visual_Dragger_op_Equality.md) |  |
|  | [Inequality(Dragger, Dragger)](M_TFlex_Model_Model3D_Visual_Dragger_op_Inequality.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)
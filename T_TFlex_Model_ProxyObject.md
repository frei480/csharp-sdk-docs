

Руководство по T-FLEX CAD Open API

# ProxyObject - класс  
    
Класс прокси объекта

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelProxyObject [TFlex.Model.Model2DProxyObject2D](T_TFlex_Model_Model2D_ProxyObject2D.md) [TFlex.Model.Model3DProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class ProxyObject
```




Тип ProxyObject предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ProxyObject](M_TFlex_Model_ProxyObject__ctor.md) | Конструктор |
|  | [ProxyObject(IntPtr)](M_TFlex_Model_ProxyObject__ctor_1.md) | Конструктор, принимающий родительский объект |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [IconID](P_TFlex_Model_ProxyObject_IconID.md) | Идентификатор иконки прокси объекта |
|  | [IsAlwaysDrawing](P_TFlex_Model_ProxyObject_IsAlwaysDrawing.md) | Отключить кэширование рисования |
|  | [IsConstruction](P_TFlex_Model_ProxyObject_IsConstruction.md) | Определить прокси объект как элемент построения |
|  | [Owner](P_TFlex_Model_ProxyObject_Owner.md) | Владелец объекта |
|  | [OwnerApp](P_TFlex_Model_ProxyObject_OwnerApp.md) | **Устарело.** |
|  | [Plugin](P_TFlex_Model_ProxyObject_Plugin.md) | Приложение, определяющее промежуточный (прокси-) объект |
|  | [Rep](P_TFlex_Model_ProxyObject_Rep.md) |  |
|  | [TypeID](P_TFlex_Model_ProxyObject_TypeID.md) | Идентификатор типа объекта |
|  | [TypeName](P_TFlex_Model_ProxyObject_TypeName.md) | Имя типа объекта |
|  | [Version](P_TFlex_Model_ProxyObject_Version.md) | Версия прокси объекта |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDiagnosticsMessage](M_TFlex_Model_ProxyObject_AddDiagnosticsMessage.md) | Добавить диагностическое сообщение. Надо вызывать из Draw |
|  | [AdjustPopupToolBarButtonSet](M_TFlex_Model_ProxyObject_AdjustPopupToolBarButtonSet.md) |  |
|  | [CanAddDiagnosticsMessage](M_TFlex_Model_ProxyObject_CanAddDiagnosticsMessage.md) | Можно ли добавить диагностическое сообщение. |
|  | [Clone](M_TFlex_Model_ProxyObject_Clone.md) | Метод создает неполную копию прокси объекта |
|  | [Draw(Graphics)](M_TFlex_Model_ProxyObject_Draw.md) | Метод для прорисовки объекта |
|  | [Draw(ProxyObjectDrawContext)](M_TFlex_Model_ProxyObject_Draw_1.md) | Метод для прорисовки объекта |
|  | [Edit](M_TFlex_Model_ProxyObject_Edit.md) | Виртуальный метод изменения прокси объекта |
|  | [EditProperties](M_TFlex_Model_ProxyObject_EditProperties.md) | Метод для редактирования свойств прокси объекта |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Equals(ProxyObject)](M_TFlex_Model_ProxyObject_Equals.md) | Метод выполняет сравнение прокси объекта ProxyObject с исходным |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetContextMenu](M_TFlex_Model_ProxyObject_GetContextMenu.md) | Метод вызывается при вызове контекстного меню прокси объекта |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetMarkObjects](M_TFlex_Model_ProxyObject_GetMarkObjects.md) | Получить список дополнительных объектов для пометки при выборе |
|  | [GetNode](M_TFlex_Model_ProxyObject_GetNode.md) | Получить координаты узла привязки по ID |
|  | [GetNodeCount](M_TFlex_Model_ProxyObject_GetNodeCount.md) | Получить количество узлов в модели |
|  | [GetNodeID](M_TFlex_Model_ProxyObject_GetNodeID.md) | Получить идентификатор узла по номеру |
|  | [GetPropList](M_TFlex_Model_ProxyObject_GetPropList.md) | Получить массив свойств |
|  | [GetRealProp](M_TFlex_Model_ProxyObject_GetRealProp.md) | Получить значение свойства с действительным значением по имени |
|  | [GetTextProp](M_TFlex_Model_ProxyObject_GetTextProp.md) | Получить значение текстового свойства по имени |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IsReallyChanged](M_TFlex_Model_ProxyObject_IsReallyChanged.md) | изменился ли в действительности прокси объект |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCommand](M_TFlex_Model_ProxyObject_OnCommand.md) | Метод для обработки команд контекстного меню |
|  | [OnDelete](M_TFlex_Model_ProxyObject_OnDelete.md) | Событие возникающее при удалении прокси объекта |
|  | [OnUndoAction](M_TFlex_Model_ProxyObject_OnUndoAction.md) | Обработчик события отмены |
|  | [Read](M_TFlex_Model_ProxyObject_Read.md) | Метод для считывания данных прокси объекта из файла |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Write](M_TFlex_Model_ProxyObject_Write.md) | Метод для записи данных прокси объекта в файл |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
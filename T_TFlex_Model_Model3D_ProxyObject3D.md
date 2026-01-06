

Руководство по T-FLEX CAD Open API

# ProxyObject3D - класс  
    
Базовый класс для 3D объектов внешнего приложения, встраиваемых в модель

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelProxyObject](T_TFlex_Model_ProxyObject.md) TFlex.Model.Model3DProxyObject3D [TFlex.Model.Model3DProxyOperation](T_TFlex_Model_Model3D_ProxyOperation.md)

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class ProxyObject3D : ProxyObject
```
```vb
Public MustInherit Class ProxyObject3D
	Inherits ProxyObject
```
```cpp
public ref class ProxyObject3D abstract : public ProxyObject
```


Тип ProxyObject3D предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ProxyObject3D](M_TFlex_Model_Model3D_ProxyObject3D__ctor.md) | Инициализирует новый экземпляр класса ProxyObject3D |
|  | [ProxyObject3D(IntPtr)](M_TFlex_Model_Model3D_ProxyObject3D__ctor_1.md) | Инициализирует новый экземпляр класса ProxyObject3D |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [IconID](P_TFlex_Model_ProxyObject_IconID.md) | Идентификатор иконки прокси объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [IsAlwaysDrawing](P_TFlex_Model_ProxyObject_IsAlwaysDrawing.md) | Отключить кэширование рисования(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [IsConstruction](P_TFlex_Model_ProxyObject_IsConstruction.md) | Определить прокси объект как элемент построения(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Owner](P_TFlex_Model_ProxyObject_Owner.md) | Владелец объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [OwnerApp](P_TFlex_Model_ProxyObject_OwnerApp.md) | **Устарело.**(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Plugin](P_TFlex_Model_ProxyObject_Plugin.md) | Приложение, определяющее промежуточный (прокси-) объект(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Rep](P_TFlex_Model_ProxyObject_Rep.md) | (Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [TypeID](P_TFlex_Model_ProxyObject_TypeID.md) | Идентификатор типа объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [TypeName](P_TFlex_Model_ProxyObject_TypeName.md) | Имя типа объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Version](P_TFlex_Model_ProxyObject_Version.md) | Версия прокси объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDiagnosticsMessage](M_TFlex_Model_ProxyObject_AddDiagnosticsMessage.md) | Добавить диагностическое сообщение. Надо вызывать из Draw(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [AdjustPopupToolBarButtonSet](M_TFlex_Model_ProxyObject_AdjustPopupToolBarButtonSet.md) | (Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [CanAddDiagnosticsMessage](M_TFlex_Model_ProxyObject_CanAddDiagnosticsMessage.md) | Можно ли добавить диагностическое сообщение.(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Clone](M_TFlex_Model_ProxyObject_Clone.md) | Метод создает неполную копию прокси объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Draw(Graphics)](M_TFlex_Model_ProxyObject_Draw.md) | Метод для прорисовки объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Draw(ProxyObjectDrawContext)](M_TFlex_Model_ProxyObject_Draw_1.md) | Метод для прорисовки объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Edit](M_TFlex_Model_ProxyObject_Edit.md) | Виртуальный метод изменения прокси объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [EditProperties](M_TFlex_Model_ProxyObject_EditProperties.md) | Метод для редактирования свойств прокси объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Equals(ProxyObject)](M_TFlex_Model_ProxyObject_Equals.md) | Метод выполняет сравнение прокси объекта [ProxyObject](T_TFlex_Model_ProxyObject.md) с исходным(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetContextMenu](M_TFlex_Model_ProxyObject_GetContextMenu.md) | Метод вызывается при вызове контекстного меню прокси объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetMarkObjects](M_TFlex_Model_ProxyObject_GetMarkObjects.md) | Получить список дополнительных объектов для пометки при выборе(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetNode](M_TFlex_Model_ProxyObject_GetNode.md) | Получить координаты узла привязки по ID(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetNodeCount](M_TFlex_Model_ProxyObject_GetNodeCount.md) | Получить количество узлов в модели(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetNodeID](M_TFlex_Model_ProxyObject_GetNodeID.md) | Получить идентификатор узла по номеру(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetPropList](M_TFlex_Model_ProxyObject_GetPropList.md) | Получить массив свойств(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetRealProp](M_TFlex_Model_ProxyObject_GetRealProp.md) | Получить значение свойства с действительным значением по имени(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetTextProp](M_TFlex_Model_ProxyObject_GetTextProp.md) | Получить значение текстового свойства по имени(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IsReallyChanged](M_TFlex_Model_ProxyObject_IsReallyChanged.md) | изменился ли в действительности прокси объект(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCommand](M_TFlex_Model_ProxyObject_OnCommand.md) | Метод для обработки команд контекстного меню(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [OnDelete](M_TFlex_Model_ProxyObject_OnDelete.md) | Событие возникающее при удалении прокси объекта(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [OnUndoAction](M_TFlex_Model_ProxyObject_OnUndoAction.md) | Обработчик события отмены(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [Read](M_TFlex_Model_ProxyObject_Read.md) | Метод для считывания данных прокси объекта из файла(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Write](M_TFlex_Model_ProxyObject_Write.md) | Метод для записи данных прокси объекта в файл(Унаследован от [ProxyObject](T_TFlex_Model_ProxyObject.md)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
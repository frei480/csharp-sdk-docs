

Руководство по T-FLEX CAD Open API

# GeometrySelectionFilter - класс  
    
Фильтр, позволяющий выбирать или не выбирать геометрию объектов

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelSelectionFilter](T_TFlex_Model_SelectionFilter.md) [TFlex.ModelCustomFilter](T_TFlex_Model_CustomFilter.md) TFlex.CommandGeometrySelectionFilter

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public class GeometrySelectionFilter : CustomFilter
```
```vb
Public Class GeometrySelectionFilter
	Inherits CustomFilter
```
```cpp
public ref class GeometrySelectionFilter : public CustomFilter
```


Тип GeometrySelectionFilter предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [GeometrySelectionFilter](M_TFlex_Command_GeometrySelectionFilter__ctor.md) | Конструктор. По умолчанию устанавливается выбор всех типов объектов и геометрии |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CanSelectObject](M_TFlex_Command_GeometrySelectionFilter_CanSelectObject.md) | (Переопределяет [CustomFilterCanSelectObject(ModelObject)](M_TFlex_Model_CustomFilter_CanSelectObject.md)) |
|  | [CanSelectType](M_TFlex_Command_GeometrySelectionFilter_CanSelectType.md) | (Переопределяет [CustomFilterCanSelectType(ObjectType)](M_TFlex_Model_CustomFilter_CanSelectType.md)) |
|  | [Disable(ObjectType)](M_TFlex_Model_SelectionFilter_Disable.md) | Запретить выбор объектов указанного типа(Унаследован от [SelectionFilter](T_TFlex_Model_SelectionFilter.md)) |
|  | [Disable(SelectableGeometryType)](M_TFlex_Command_GeometrySelectionFilter_Disable.md) | Запретить выбор геометрии указанного типа |
|  | [DisableAllTypes](M_TFlex_Model_SelectionFilter_DisableAllTypes.md) | Выключить выбор объектов всех типов(Унаследован от [SelectionFilter](T_TFlex_Model_SelectionFilter.md)) |
|  | [DisableAllTypesImpl](M_TFlex_Command_GeometrySelectionFilter_DisableAllTypesImpl.md) | (Переопределяет [SelectionFilterDisableAllTypesImpl](M_TFlex_Model_SelectionFilter_DisableAllTypesImpl.md)) |
|  | [DisableImpl](M_TFlex_Command_GeometrySelectionFilter_DisableImpl.md) | (Переопределяет [SelectionFilterDisableImpl(ObjectType)](M_TFlex_Model_SelectionFilter_DisableImpl.md)) |
|  | [Dispose](M_TFlex_Model_SelectionFilter_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [SelectionFilter](T_TFlex_Model_SelectionFilter.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_SelectionFilter_Dispose_1.md) | (Унаследован от [SelectionFilter](T_TFlex_Model_SelectionFilter.md)) |
|  | [Enable(ObjectType)](M_TFlex_Model_SelectionFilter_Enable.md) | Разрешить выбор объектов указанного типа(Унаследован от [SelectionFilter](T_TFlex_Model_SelectionFilter.md)) |
|  | [Enable(SelectableGeometryType)](M_TFlex_Command_GeometrySelectionFilter_Enable.md) | Разрешить выбор геометрии указанного типа |
|  | [EnableAllTypes](M_TFlex_Model_SelectionFilter_EnableAllTypes.md) | Включить выбор объектов любых типов(Унаследован от [SelectionFilter](T_TFlex_Model_SelectionFilter.md)) |
|  | [EnableAllTypesImpl](M_TFlex_Command_GeometrySelectionFilter_EnableAllTypesImpl.md) | (Переопределяет [SelectionFilterEnableAllTypesImpl](M_TFlex_Model_SelectionFilter_EnableAllTypesImpl.md)) |
|  | [EnableImpl](M_TFlex_Command_GeometrySelectionFilter_EnableImpl.md) | (Переопределяет [SelectionFilterEnableImpl(ObjectType)](M_TFlex_Model_SelectionFilter_EnableImpl.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Model_SelectionFilter_Finalize.md) | (Унаследован от [SelectionFilter](T_TFlex_Model_SelectionFilter.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Command - пространство имён](N_TFlex_Command.md)
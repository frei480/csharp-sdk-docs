

Руководство по T-FLEX CAD Open API

# BasePipeBorderInfo - класс  
  
---  
  
Класс описывает границу трубопровода

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DBasePipeBorderInfo

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class BorderInfo
```
```vb
Public Class BorderInfo
```
```cpp
public ref class BorderInfo
```


Тип BasePipeBorderInfo предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Offset](P_TFlex_Model_Model3D_BasePipe_BorderInfo_Offset.md) | Полное значение смещения границы трубопровода в единицах пользователя |
|  | [Point](P_TFlex_Model_Model3D_BasePipe_BorderInfo_Point.md) | Добавить / удалить геометрическое смещение границы трубопровода, допустимо заначени null. Все предыдущие параметрические и геометрические смещения будут удалены. |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddOffset](M_TFlex_Model_Model3D_BasePipe_BorderInfo_AddOffset.md) | Добавить параметрическое смещение границы трубопровода |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetOffsetList](M_TFlex_Model_Model3D_BasePipe_BorderInfo_GetOffsetList.md) |  |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveOffset](M_TFlex_Model_Model3D_BasePipe_BorderInfo_RemoveOffset.md) | Удалить все параметрические смещения границы трубопровода |
|  | [Reset](M_TFlex_Model_Model3D_BasePipe_BorderInfo_Reset.md) | Сбросить границу в значение по умолчанию, конечная граница в конце пути, начальная граница в начале |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
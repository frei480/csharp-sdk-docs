

Руководство по T-FLEX CAD Open API

# ExportTo3dCommon - класс  
  
---  
  
Базовый класс для экспорта в некоторые универсальные 3D форматы(STEP, ACIS, JT, PRC, 3MF, IGES, GLTF)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) TFlex.ModelExportTo3dCommon Подробнее

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class ExportTo3dCommon : ExportTo
```
```vb
Public MustInherit Class ExportTo3dCommon
	Inherits ExportTo
```
```cpp
public ref class ExportTo3dCommon abstract : public ExportTo
```


Тип ExportTo3dCommon предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ExportTo3dCommon](M_TFlex_Model_ExportTo3dCommon__ctor.md) | Инициализирует новый экземпляр класса ExportTo3dCommon |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ColorSource](P_TFlex_Model_ExportTo3dCommon_ColorSource.md) | Источник для цвета |
|  | [Export3DNodes](P_TFlex_Model_ExportTo3dCommon_Export3DNodes.md) | Экспортировать 3д узлы |
|  | [Export3DPictures](P_TFlex_Model_ExportTo3dCommon_Export3DPictures.md) | Экспортировать 3D изображения |
|  | [ExportAnotation](P_TFlex_Model_ExportTo3dCommon_ExportAnotation.md) | Экспортировать аннотации |
|  | [ExportContours](P_TFlex_Model_ExportTo3dCommon_ExportContours.md) | Экспортировать профили |
|  | [ExportCurves](P_TFlex_Model_ExportTo3dCommon_ExportCurves.md) | Экспортировать кривые |
|  | [ExportSheetBodies](P_TFlex_Model_ExportTo3dCommon_ExportSheetBodies.md) | Экспортировать листовые тела |
|  | [ExportSolidBodies](P_TFlex_Model_ExportTo3dCommon_ExportSolidBodies.md) | Экспортировать твёрдые тела |
|  | [ExportWelds](P_TFlex_Model_ExportTo3dCommon_ExportWelds.md) | Экспортировать сварные швы |
|  | [ExportWireBodies](P_TFlex_Model_ExportTo3dCommon_ExportWireBodies.md) | Экспортировать проволочные тела(кривые) |
|  | [Mode](P_TFlex_Model_ExportTo3dCommon_Mode.md) | Тип экспорта |
|  | [ShowDialog](P_TFlex_Model_ExportTo3dCommon_ShowDialog.md) | Показывать диалог опций импорта |
|  | [SimplifyGeometry](P_TFlex_Model_ExportTo3dCommon_SimplifyGeometry.md) | Упрощать геометрию |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AdvancedFormatOptions](M_TFlex_Model_ExportTo3dCommon_AdvancedFormatOptions.md) |  |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Export](M_TFlex_Model_ExportTo3dCommon_Export.md) | Функция экспорта в файл(Переопределяет [ExportToExport(String)](M_TFlex_Model_ExportTo_Export.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Format](M_TFlex_Model_ExportTo3dCommon_Format.md) |  |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) TFlex.ModelExportTo3dCommon [TFlex.ModelExportTo3mf](T_TFlex_Model_ExportTo3mf.md) [TFlex.ModelExportToAcis](T_TFlex_Model_ExportToAcis.md) [TFlex.ModelExportToGltf](T_TFlex_Model_ExportToGltf.md) [TFlex.ModelExportToIges](T_TFlex_Model_ExportToIges.md) [TFlex.ModelExportToJt](T_TFlex_Model_ExportToJt.md) [TFlex.ModelExportToPrc](T_TFlex_Model_ExportToPrc.md) [TFlex.ModelExportToStep](T_TFlex_Model_ExportToStep.md)
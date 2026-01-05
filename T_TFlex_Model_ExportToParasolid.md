

Руководство по T-FLEX CAD Open API

# ExportToParasolid - класс  
  
---  
  
Класс экспорта в файлы форматов Parasolid

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) TFlex.ModelExportToParasolid

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ExportToParasolid : ExportTo
```
```vb
Public NotInheritable Class ExportToParasolid
	Inherits ExportTo
```
```cpp
public ref class ExportToParasolid sealed : public ExportTo
```


Тип ExportToParasolid предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ExportToParasolid](M_TFlex_Model_ExportToParasolid__ctor.md) | Инициализирует новый экземпляр класса ExportToParasolid |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ColorSource](P_TFlex_Model_ExportToParasolid_ColorSource.md) | Источник для цвета |
|  | [CompanyName](P_TFlex_Model_ExportToParasolid_CompanyName.md) | Название экспортирующей компании |
|  | [ConverterName](P_TFlex_Model_ExportToParasolid_ConverterName.md) | Название конвертера |
|  | [CopyArraysGeometry](P_TFlex_Model_ExportToParasolid_CopyArraysGeometry.md) | Копировать геометрию массивов |
|  | [DeleteRedundant](P_TFlex_Model_ExportToParasolid_DeleteRedundant.md) | Удалить избыточную геометрию |
|  | [ExportContours](P_TFlex_Model_ExportToParasolid_ExportContours.md) | Экспортировать профили |
|  | [ExportCurves](P_TFlex_Model_ExportToParasolid_ExportCurves.md) | Экспортировать кривые |
|  | [ExportPaths3D](P_TFlex_Model_ExportToParasolid_ExportPaths3D.md) | Экспортировать 3D пути |
|  | [ExportSheetBodies](P_TFlex_Model_ExportToParasolid_ExportSheetBodies.md) | Экспортировать листовые тела |
|  | [ExportSolidBodies](P_TFlex_Model_ExportToParasolid_ExportSolidBodies.md) | Экспортировать твёрдые тела |
|  | [ExportWelds](P_TFlex_Model_ExportToParasolid_ExportWelds.md) | Экспортировать сварные швы |
|  | [ExportWireBodies](P_TFlex_Model_ExportToParasolid_ExportWireBodies.md) | Экспортировать проволочные тела(кривые) |
|  | [FileFormat](P_TFlex_Model_ExportToParasolid_FileFormat.md) | Формат файла |
|  | [FileVersion](P_TFlex_Model_ExportToParasolid_FileVersion.md) | **Устарело.** Версия выходного файла |
|  | [Mode](P_TFlex_Model_ExportToParasolid_Mode.md) | Тип экспорта |
|  | [ModelName](P_TFlex_Model_ExportToParasolid_ModelName.md) | Название модели |
|  | [ParasolidVersion](P_TFlex_Model_ExportToParasolid_ParasolidVersion.md) | Версия |
|  | [ShowDialog](P_TFlex_Model_ExportToParasolid_ShowDialog.md) | Показывать диалог опций экспорта |
|  | [SystemName](P_TFlex_Model_ExportToParasolid_SystemName.md) | Название экспортирующей системы |
|  | [UserName](P_TFlex_Model_ExportToParasolid_UserName.md) | Имя пользователя |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Export](M_TFlex_Model_ExportToParasolid_Export.md) | Функция экспорта документа(Переопределяет [ExportToExport(String)](M_TFlex_Model_ExportTo_Export.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
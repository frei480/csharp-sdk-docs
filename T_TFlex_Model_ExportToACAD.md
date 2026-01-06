

Руководство по T-FLEX CAD Open API

# ExportToACAD - класс  
    
Класс экспорта в форматы AutoCAD

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) TFlex.ModelExportToACAD [TFlex.ModelExportToDWG](T_TFlex_Model_ExportToDWG.md) [TFlex.ModelExportToDXB](T_TFlex_Model_ExportToDXB.md) [TFlex.ModelExportToDXF](T_TFlex_Model_ExportToDXF.md) [TFlex.ModelExportToDXF3D](T_TFlex_Model_ExportToDXF3D.md)

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public abstract class ExportToACAD : ExportTo
```




Тип ExportToACAD предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AutocadExportFileVersion](P_TFlex_Model_ExportToACAD_AutocadExportFileVersion.md) | Установка версии файла Autocad |
|  | [BiarcInterpolationAccuracyForSplines](P_TFlex_Model_ExportToACAD_BiarcInterpolationAccuracyForSplines.md) | Точность круговой интерполяции |
|  | [BiarcInterpolationForSplines](P_TFlex_Model_ExportToACAD_BiarcInterpolationForSplines.md) | Экспортировать сплайны с использованием круговой интерполяции |
|  | [ConvertAreas](P_TFlex_Model_ExportToACAD_ConvertAreas.md) | Конвертировать штриховки: true - в штриховки, false - в линии |
|  | [ConvertDimensions](P_TFlex_Model_ExportToACAD_ConvertDimensions.md) | Конвертировать размеры: 0 - в размеры, 1 - в размеры и тексты, 2 - в линии и тексты |
|  | [ConvertLineText](P_TFlex_Model_ExportToACAD_ConvertLineText.md) | Конвертировать строчные тексты: false - в тексты, true - в линии |
|  | [ConvertMultitext](P_TFlex_Model_ExportToACAD_ConvertMultitext.md) | Конвертировать мультитексты: 0 - выборочно, 1 - в мультитексты, 2 - в тексты и линии |
|  | [ConvertToLines](P_TFlex_Model_ExportToACAD_ConvertToLines.md) | Конвертировать линии: true - в линии, false - в полилинии |
|  | [ExportAllPages](P_TFlex_Model_ExportToACAD_ExportAllPages.md) | Экспортировать все страницы |
|  | [ExportPages](P_TFlex_Model_ExportToACAD_ExportPages.md) | Экспортируемые страницы |
|  | [FileVersion](P_TFlex_Model_ExportToACAD_FileVersion.md) | **Устарело.** |
|  | [NotCreateBlocksForPages](P_TFlex_Model_ExportToACAD_NotCreateBlocksForPages.md) | Не создавать блоки для страниц |
|  | [OrientPagesInModelSpace](P_TFlex_Model_ExportToACAD_OrientPagesInModelSpace.md) |  |
|  | [Page](P_TFlex_Model_ExportToACAD_Page.md) | Установить экспортируемую страницу |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Export](M_TFlex_Model_ExportTo_Export.md) | Функция экспорта документа(Унаследован от [ExportTo](T_TFlex_Model_ExportTo.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
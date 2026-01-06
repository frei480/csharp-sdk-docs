

Руководство по T-FLEX CAD Open API

# ExportToDXF3D - класс  
    
Класс экспорта в файл форматa DXF 3D

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) [TFlex.ModelExportToACAD](T_TFlex_Model_ExportToACAD.md) TFlex.ModelExportToDXF3D

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class ExportToDXF3D : ExportToACAD
```




Тип ExportToDXF3D предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ExportToDXF3D](M_TFlex_Model_ExportToDXF3D__ctor.md) | Инициализирует новый экземпляр класса ExportToDXF3D |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AngleTolerance](P_TFlex_Model_ExportToDXF3D_AngleTolerance.md) | Допуск по углу |
|  | [AutocadExportFileVersion](P_TFlex_Model_ExportToACAD_AutocadExportFileVersion.md) | Установка версии файла Autocad(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [BiarcInterpolationAccuracyForSplines](P_TFlex_Model_ExportToACAD_BiarcInterpolationAccuracyForSplines.md) | Точность круговой интерполяции(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [BiarcInterpolationForSplines](P_TFlex_Model_ExportToACAD_BiarcInterpolationForSplines.md) | Экспортировать сплайны с использованием круговой интерполяции(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [ConvertAreas](P_TFlex_Model_ExportToACAD_ConvertAreas.md) | Конвертировать штриховки: true - в штриховки, false - в линии(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [ConvertDimensions](P_TFlex_Model_ExportToACAD_ConvertDimensions.md) | Конвертировать размеры: 0 - в размеры, 1 - в размеры и тексты, 2 - в линии и тексты(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [ConvertLineText](P_TFlex_Model_ExportToACAD_ConvertLineText.md) | Конвертировать строчные тексты: false - в тексты, true - в линии(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [ConvertMultitext](P_TFlex_Model_ExportToACAD_ConvertMultitext.md) | Конвертировать мультитексты: 0 - выборочно, 1 - в мультитексты, 2 - в тексты и линии(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [ConvertToLines](P_TFlex_Model_ExportToACAD_ConvertToLines.md) | Конвертировать линии: true - в линии, false - в полилинии(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [EdgeTolerance](P_TFlex_Model_ExportToDXF3D_EdgeTolerance.md) | Допуск по ребру |
|  | [ExportAllPages](P_TFlex_Model_ExportToACAD_ExportAllPages.md) | Экспортировать все страницы(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [ExportPages](P_TFlex_Model_ExportToACAD_ExportPages.md) | Экспортируемые страницы(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [FaceTolerance](P_TFlex_Model_ExportToDXF3D_FaceTolerance.md) | Точность грани |
|  | [FileVersion](P_TFlex_Model_ExportToDXF3D_FileVersion.md) | Версия выходного файла |
|  | [LayerModel](P_TFlex_Model_ExportToDXF3D_LayerModel.md) | Цветовая модель для экспорта в STL |
|  | [LinearTolerance](P_TFlex_Model_ExportToDXF3D_LinearTolerance.md) | **Устарело.** Допуск |
|  | [MaxCellSize](P_TFlex_Model_ExportToDXF3D_MaxCellSize.md) | **Устарело.** Максимальный размер ячейки |
|  | [NormalTolerance](P_TFlex_Model_ExportToDXF3D_NormalTolerance.md) | **Устарело.** Максимальное уклонение нормали |
|  | [NotCreateBlocksForPages](P_TFlex_Model_ExportToACAD_NotCreateBlocksForPages.md) | Не создавать блоки для страниц(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [OrientPagesInModelSpace](P_TFlex_Model_ExportToACAD_OrientPagesInModelSpace.md) | (Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
|  | [Page](P_TFlex_Model_ExportToACAD_Page.md) | Установить экспортируемую страницу(Унаследован от [ExportToACAD](T_TFlex_Model_ExportToACAD.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Export](M_TFlex_Model_ExportToDXF3D_Export.md) | Функция экспорта документа(Переопределяет [ExportToExport(String)](M_TFlex_Model_ExportTo_Export.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
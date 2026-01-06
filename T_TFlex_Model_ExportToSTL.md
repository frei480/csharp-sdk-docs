

Руководство по T-FLEX CAD Open API

# ExportToSTL - класс  
    
Класс экспорта в файл формата STL

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) [TFlex.ModelExportToFacet](T_TFlex_Model_ExportToFacet.md) TFlex.ModelExportToSTL

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ExportToSTL : ExportToFacet
```




Тип ExportToSTL предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ExportToSTL](M_TFlex_Model_ExportToSTL__ctor.md) | Инициализирует новый экземпляр класса ExportToSTL |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AngleTolerance](P_TFlex_Model_ExportToFacet_AngleTolerance.md) | Допуск по углу(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [Binary](P_TFlex_Model_ExportToSTL_Binary.md) | Использовать бинарный формат STL |
|  | [ColorModel](P_TFlex_Model_ExportToSTL_ColorModel.md) | Цветовая модель для экспорта в STL |
|  | [DivideByOperation](P_TFlex_Model_ExportToSTL_DivideByOperation.md) | Писать отдельный файл для каждой операции |
|  | [EdgeTolerance](P_TFlex_Model_ExportToFacet_EdgeTolerance.md) | Допуск по ребру(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [Facet](P_TFlex_Model_ExportToFacet_Facet.md) | Качество сетки(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [FaceTolerance](P_TFlex_Model_ExportToFacet_FaceTolerance.md) | Точность грани(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [LinearTolerance](P_TFlex_Model_ExportToSTL_LinearTolerance.md) | **Устарело.** Допуск |
|  | [MaxCellSize](P_TFlex_Model_ExportToSTL_MaxCellSize.md) | **Устарело.** Максимальный размер ячейки |
|  | [NormalTolerance](P_TFlex_Model_ExportToSTL_NormalTolerance.md) | **Устарело.** Максимальное уклонение нормали |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Export](M_TFlex_Model_ExportToSTL_Export.md) | Функция экспорта документа(Переопределяет [ExportToFacetExport(String)](M_TFlex_Model_ExportToFacet_Export.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
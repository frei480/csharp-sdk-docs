

Руководство по T-FLEX CAD Open API

# ExportToInventor - класс  
    
Класс экспорта в файл форматa Open Inventor

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) [TFlex.ModelExportToFacet](T_TFlex_Model_ExportToFacet.md) TFlex.ModelExportToInventor

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ExportToInventor : ExportToFacet
```
```vb
Public NotInheritable Class ExportToInventor
	Inherits ExportToFacet
```
```cpp
public ref class ExportToInventor sealed : public ExportToFacet
```


Тип ExportToInventor предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ExportToInventor](M_TFlex_Model_ExportToInventor__ctor.md) | Инициализирует новый экземпляр класса ExportToInventor |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AngleTolerance](P_TFlex_Model_ExportToFacet_AngleTolerance.md) | Допуск по углу(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [EdgeTolerance](P_TFlex_Model_ExportToFacet_EdgeTolerance.md) | Допуск по ребру(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [ExportTFLEXData](P_TFlex_Model_ExportToInventor_ExportTFLEXData.md) | Экспортировать данные, необходимые для вставки данного файла в T-FLEX CAD |
|  | [Facet](P_TFlex_Model_ExportToFacet_Facet.md) | Качество сетки(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [FaceTolerance](P_TFlex_Model_ExportToFacet_FaceTolerance.md) | Точность грани(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Export](M_TFlex_Model_ExportToInventor_Export.md) | Функция экспорта документа(Переопределяет [ExportToFacetExport(String)](M_TFlex_Model_ExportToFacet_Export.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
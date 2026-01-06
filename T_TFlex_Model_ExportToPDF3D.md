

Руководство по T-FLEX CAD Open API

# ExportToPDF3D - класс  
    
Класс экспорта в файл форматa PDF3D

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelExportTo](T_TFlex_Model_ExportTo.md) [TFlex.ModelExportToFacet](T_TFlex_Model_ExportToFacet.md) TFlex.ModelExportToPDF3D

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ExportToPDF3D : ExportToFacet
```
```vb
Public NotInheritable Class ExportToPDF3D
	Inherits ExportToFacet
```
```cpp
public ref class ExportToPDF3D sealed : public ExportToFacet
```


Тип ExportToPDF3D предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ExportToPDF3D](M_TFlex_Model_ExportToPDF3D__ctor.md) | Инициализирует новый экземпляр класса ExportToPDF3D |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AngleTolerance](P_TFlex_Model_ExportToFacet_AngleTolerance.md) | Допуск по углу(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [Attributes](P_TFlex_Model_ExportToPDF3D_Attributes.md) | Экспортировать атрибуты |
|  | [Edges](P_TFlex_Model_ExportToPDF3D_Edges.md) | Экспортировать рёбра |
|  | [EdgeTolerance](P_TFlex_Model_ExportToFacet_EdgeTolerance.md) | Допуск по ребру(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [ExportDecorations](P_TFlex_Model_ExportToPDF3D_ExportDecorations.md) | Экспорт элементов 3D оформления |
|  | [ExportLightSources](P_TFlex_Model_ExportToPDF3D_ExportLightSources.md) | Экспорт источников света |
|  | [Facet](P_TFlex_Model_ExportToFacet_Facet.md) | Качество сетки(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [FaceTolerance](P_TFlex_Model_ExportToFacet_FaceTolerance.md) | Точность грани(Унаследован от [ExportToFacet](T_TFlex_Model_ExportToFacet.md)) |
|  | [Layers](P_TFlex_Model_ExportToPDF3D_Layers.md) | Экспортировать слои. Слои экспортируются как узлы дерева модели |
|  | [Material](P_TFlex_Model_ExportToPDF3D_Material.md) | Экспортировать с материалами |
|  | [OpenExportFile](P_TFlex_Model_ExportToPDF3D_OpenExportFile.md) | Открывать файл после экспорта |
|  | [Texture](P_TFlex_Model_ExportToPDF3D_Texture.md) | Экспортировать с текстурами. Опция экспорта с материалами должна быть включена |
|  | [TreeModel](P_TFlex_Model_ExportToPDF3D_TreeModel.md) | Экспортировать дерево модели |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Export](M_TFlex_Model_ExportToPDF3D_Export.md) | Функция экспорта документа(Переопределяет [ExportToFacetExport(String)](M_TFlex_Model_ExportToFacet_Export.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
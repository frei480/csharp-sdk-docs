

Руководство по T-FLEX CAD Open API

# ImportFrom3dCommon - класс  
  
---  
  
Класс импорта из множества популярных форматов CAD-систем(step, acis, iges, SolidWorks, NX, SolidEdge, Creo,...)

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelImportFrom3dCommon

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ImportFrom3dCommon
```
```vb
Public NotInheritable Class ImportFrom3dCommon
```
```cpp
public ref class ImportFrom3dCommon sealed
```


Тип ImportFrom3dCommon предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ImportFrom3dCommon](M_TFlex_Model_ImportFrom3dCommon__ctor.md) | Инициализирует новый экземпляр класса ImportFrom3dCommon |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddBodyRecordsInProductStructure](P_TFlex_Model_ImportFrom3dCommon_AddBodyRecordsInProductStructure.md) | Добавить записи о телах в структуру изделия |
|  | [CheckImportGeomerty](P_TFlex_Model_ImportFrom3dCommon_CheckImportGeomerty.md) | Сделать проверку тел, после импорта |
|  | [CreateAccurateEdges](P_TFlex_Model_ImportFrom3dCommon_CreateAccurateEdges.md) | Строить точные рёбра |
|  | [CreateAssociativeLinks](P_TFlex_Model_ImportFrom3dCommon_CreateAssociativeLinks.md) | Создавать ассоциативные связи |
|  | [DefaultAnnotationFontName](P_TFlex_Model_ImportFrom3dCommon_DefaultAnnotationFontName.md) | Выбор шрифта по умолчанию для текста |
|  | [DefaultUnit](P_TFlex_Model_ImportFrom3dCommon_DefaultUnit.md) | Единица измерения по умолчанию |
|  | [DocumentPrototypePath](P_TFlex_Model_ImportFrom3dCommon_DocumentPrototypePath.md) | Путь к документу, который используется в качестве прототипа |
|  | [Heal](P_TFlex_Model_ImportFrom3dCommon_Heal.md) | Лечение геометрии |
|  | [ImportAnotations](P_TFlex_Model_ImportFrom3dCommon_ImportAnotations.md) | Импортировать аннотации |
|  | [ImportHideBodies](P_TFlex_Model_ImportFrom3dCommon_ImportHideBodies.md) | Импортировать скрытые тела |
|  | [ImportLayers](P_TFlex_Model_ImportFrom3dCommon_ImportLayers.md) | Импортировать слои |
|  | [ImportMeshBodies](P_TFlex_Model_ImportFrom3dCommon_ImportMeshBodies.md) | Импортировать сеточные тела в виде 3D изображений |
|  | [ImportOnlyFromActiveFilter](P_TFlex_Model_ImportFrom3dCommon_ImportOnlyFromActiveFilter.md) | Импортировать тела только с активного слоя |
|  | [ImportSheetBodies](P_TFlex_Model_ImportFrom3dCommon_ImportSheetBodies.md) | Импортировать листовые тела |
|  | [ImportSolidBodies](P_TFlex_Model_ImportFrom3dCommon_ImportSolidBodies.md) | Импортировать твёрдые тела |
|  | [ImportWireBodies](P_TFlex_Model_ImportFrom3dCommon_ImportWireBodies.md) | Импортировать проволочные тела(кривые) |
|  | [OverrideAnnotationFont](P_TFlex_Model_ImportFrom3dCommon_OverrideAnnotationFont.md) | Переопределить шрифт |
|  | [PathToAssemblyFolder](P_TFlex_Model_ImportFrom3dCommon_PathToAssemblyFolder.md) | Путь к папке, в которую будут сохраняться создаваемые фрагменты в режиме сборки(используются только для типа импорта - сборка) |
|  | [RecognizeAnnotation](P_TFlex_Model_ImportFrom3dCommon_RecognizeAnnotation.md) | Распозновать элементы оформления |
|  | [Sewing](P_TFlex_Model_ImportFrom3dCommon_Sewing.md) | Сшивка |
|  | [SewTolerance](P_TFlex_Model_ImportFrom3dCommon_SewTolerance.md) | Точность сшивки в мм |
|  | [ShowDialog](P_TFlex_Model_ImportFrom3dCommon_ShowDialog.md) | Показывать диалог опций импорта |
|  | [SimplifyGeometry](P_TFlex_Model_ImportFrom3dCommon_SimplifyGeometry.md) | Упрощать геометрию |
|  | [UpdateProductStructure](P_TFlex_Model_ImportFrom3dCommon_UpdateProductStructure.md) | Обновить структуру изделия |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Import](M_TFlex_Model_ImportFrom3dCommon_Import.md) | Функция импорта файла |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Configurations](F_TFlex_Model_ImportFrom3dCommon_Configurations.md) | Импортировать исполнения |
|  | [Mode](F_TFlex_Model_ImportFrom3dCommon_Mode.md) | Тип импорта |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
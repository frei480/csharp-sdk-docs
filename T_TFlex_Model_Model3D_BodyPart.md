

Руководство по T-FLEX CAD Open API

# BodyPart - класс  
  
---  
  
Класс тела в структуре модели

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DBodyPart

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class BodyPart : IDisposable
```
```vb
Public NotInheritable Class BodyPart
	Implements IDisposable
```
```cpp
public ref class BodyPart sealed : IDisposable
```


Тип BodyPart предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Active](P_TFlex_Model_Model3D_BodyPart_Active.md) | Активное тело, не использовано в как заготовка в других телах |
|  | [BaseOperation](P_TFlex_Model_Model3D_BodyPart_BaseOperation.md) | Базовая операция в теле |
|  | [CoatingMaterial](P_TFlex_Model_Model3D_BodyPart_CoatingMaterial.md) | Покрытие |
|  | [Color](P_TFlex_Model_Model3D_BodyPart_Color.md) | Цвет |
|  | [CountOperationChain](P_TFlex_Model_Model3D_BodyPart_CountOperationChain.md) | Количество операций в цепочке тела |
|  | [Facet](P_TFlex_Model_Model3D_BodyPart_Facet.md) |  |
|  | [Layer](P_TFlex_Model_Model3D_BodyPart_Layer.md) | Слой, на котором размещается объект |
|  | [Level](P_TFlex_Model_Model3D_BodyPart_Level.md) | Уровень |
|  | [Material](P_TFlex_Model_Model3D_BodyPart_Material.md) | Материал |
|  | [MeshDensity](P_TFlex_Model_Model3D_BodyPart_MeshDensity.md) | Плотность сетки в диапазоне 0.0-1.0 |
|  | [Name](P_TFlex_Model_Model3D_BodyPart_Name.md) | Имя тела |
|  | [Suppression](P_TFlex_Model_Model3D_BodyPart_Suppression.md) | Свойство подавленности операции |
|  | [TopOperation](P_TFlex_Model_Model3D_BodyPart_TopOperation.md) | Верхняя операция в теле |
|  | [UseBodyAttributes](P_TFlex_Model_Model3D_BodyPart_UseBodyAttributes.md) | Установлены атрибуты |
|  | [Virtual](P_TFlex_Model_Model3D_BodyPart_Virtual.md) | Виртуальное тело, состоит из одной операции - типа 3D фрагмент или массив(копия, симметрия) |
|  | [Wireframe](P_TFlex_Model_Model3D_BodyPart_Wireframe.md) | Признак рёберной отрисовки операции |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CreatePart](M_TFlex_Model_Model3D_BodyPart_CreatePart.md) | Создать деталь |
|  | [Dispose](M_TFlex_Model_Model3D_BodyPart_Dispose.md) | Освобождает все ресурсы, используемые объектом BodyPart |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetOperationChain](M_TFlex_Model_Model3D_BodyPart_GetOperationChain.md) | Получить операцию из цепочки тела |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Unload](M_TFlex_Model_Model3D_BodyPart_Unload.md) | Выгрузить деталь |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
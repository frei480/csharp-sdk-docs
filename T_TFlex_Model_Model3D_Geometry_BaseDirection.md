

Руководство по T-FLEX CAD Open API

# BaseDirection - класс  
    
Базовый класс для вектора

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryGeometry](T_TFlex_Model_Model3D_Geometry_Geometry.md) TFlex.Model.Model3D.GeometryBaseDirection [TFlex.Model.Model3D.GeometryDirection](T_TFlex_Model_Model3D_Geometry_Direction.md) [TFlex.Model.Model3D.GeometryModelDirection](T_TFlex_Model_Model3D_Geometry_ModelDirection.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class BaseDirection : Geometry
```




Тип BaseDirection предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Item](P_TFlex_Model_Model3D_Geometry_BaseDirection_Item.md) |  |
|  | [Magnitude](P_TFlex_Model_Model3D_Geometry_BaseDirection_Magnitude.md) | Длина вектора |
|  | [Owner](P_TFlex_Model_Model3D_Geometry_Geometry_Owner.md) | Получить модельный объект, которому принадлежит геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Reference](P_TFlex_Model_Model3D_Geometry_Geometry_Reference.md) | Создать объект типа ссылка на геометрический объект(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Valid](P_TFlex_Model_Model3D_Geometry_Geometry_Valid.md) | Проверка достоверности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [X](P_TFlex_Model_Model3D_Geometry_BaseDirection_X.md) | Получить X - координату вектора |
|  | [Y](P_TFlex_Model_Model3D_Geometry_BaseDirection_Y.md) | Получить Y - координату вектора |
|  | [Z](P_TFlex_Model_Model3D_Geometry_BaseDirection_Z.md) | Получить Z - координату вектора |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Colinear](M_TFlex_Model_Model3D_Geometry_BaseDirection_Colinear.md) | Проверить данный вектор на коллинеарность с другим |
|  | [CrossProduct](M_TFlex_Model_Model3D_Geometry_BaseDirection_CrossProduct.md) | Векторное произведение векторов |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_Geometry_Dispose_1.md) | (Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Geometry)](M_TFlex_Model_Model3D_Geometry_Geometry_Equals.md) | Проверка эквивалетности ссылки(Унаследован от [Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)) |
|  | [Equals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MakeOrtho](M_TFlex_Model_Model3D_Geometry_BaseDirection_MakeOrtho.md) | Сделать вектор, перпендикулярный данному |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [NormalizedVector](M_TFlex_Model_Model3D_Geometry_BaseDirection_NormalizedVector.md) | Нормализованный вектор |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Update](M_TFlex_Model_Model3D_Geometry_BaseDirection_Update.md) | Обновить геометрию для каждого конкретного порождённого типа(Переопределяет Geometry.Update) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Addition(BaseDirection, BaseDirection)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Addition.md) |  |
|  | [Addition(BasePoint3D, BaseDirection)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Addition_1.md) |  |
|  | [Division(BaseDirection, Double)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Division.md) |  |
|  | [Equality(BaseDirection, BaseDirection)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Equality.md) |  |
|  | [Inequality(BaseDirection, BaseDirection)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Inequality.md) |  |
|  | [Multiply(BaseDirection, Double)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Multiply.md) |  |
|  | [Multiply(BaseDirection, BaseDirection)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Multiply_1.md) |  |
|  | [Subtraction(BaseDirection, BaseDirection)](M_TFlex_Model_Model3D_Geometry_BaseDirection_op_Subtraction.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
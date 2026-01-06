

Руководство по T-FLEX CAD Open API

# TransformationMatrix - класс  
    
Базовый класс для преобразований

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryTransformationMatrix [TFlex.Model.Model3D.GeometryAffineTransformation](T_TFlex_Model_Model3D_Geometry_AffineTransformation.md)

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class TransformationMatrix
```
```vb
Public Class TransformationMatrix
```
```cpp
public ref class TransformationMatrix
```


Тип TransformationMatrix предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [TransformationMatrix](M_TFlex_Model_Model3D_Geometry_TransformationMatrix__ctor.md) | Конструктор для единичной трансформации |
|  | [TransformationMatrix(TransformationMatrix)](M_TFlex_Model_Model3D_Geometry_TransformationMatrix__ctor_1.md) | Копирующий конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Item](P_TFlex_Model_Model3D_Geometry_TransformationMatrix_Item.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetPKTransform](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_GetPKTransform.md) |  |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Identity](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_Identity.md) | Сделать матрицу единичной |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Multiply(BaseBody, TransformationMatrix)](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply.md) |  |
|  | [Multiply(BaseCurve, TransformationMatrix)](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply_1.md) |  |
|  | [Multiply(BaseDirection, TransformationMatrix)](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply_2.md) |  |
|  | [Multiply(BasePoint3D, TransformationMatrix)](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply_3.md) |  |
|  | [Multiply(BaseSurface, TransformationMatrix)](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply_4.md) |  |
|  | [Multiply(TransformationMatrix, TransformationMatrix)](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_op_Multiply_5.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
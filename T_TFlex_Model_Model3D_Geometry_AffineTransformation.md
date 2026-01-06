

Руководство по T-FLEX CAD Open API

# AffineTransformation - класс  
    
Аффинные преобразования

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.GeometryTransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md) TFlex.Model.Model3D.GeometryAffineTransformation

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class AffineTransformation : TransformationMatrix, 
	IDisposable
```
```vb
Public Class AffineTransformation
	Inherits TransformationMatrix
	Implements IDisposable
```
```cpp
public ref class AffineTransformation : public TransformationMatrix, 
	IDisposable
```


Тип AffineTransformation предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AffineTransformation](M_TFlex_Model_Model3D_Geometry_AffineTransformation__ctor.md) | Конструктор для единичной трансформации |
|  | [AffineTransformation(AffineTransformation)](M_TFlex_Model_Model3D_Geometry_AffineTransformation__ctor_1.md) | Копирующий конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Item](P_TFlex_Model_Model3D_Geometry_TransformationMatrix_Item.md) | (Унаследован от [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Geometry_AffineTransformation_Dispose.md) | Освобождает все ресурсы, используемые объектом AffineTransformation |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Geometry_AffineTransformation_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом AffineTransformation, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Model_Model3D_Geometry_AffineTransformation_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetPKTransform](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_GetPKTransform.md) | (Унаследован от [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Identity](M_TFlex_Model_Model3D_Geometry_TransformationMatrix_Identity.md) | Сделать матрицу единичной(Унаследован от [TransformationMatrix](T_TFlex_Model_Model3D_Geometry_TransformationMatrix.md)) |
|  | [Inverse](M_TFlex_Model_Model3D_Geometry_AffineTransformation_Inverse.md) | Обратная матрица |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MoveToLCS](M_TFlex_Model_Model3D_Geometry_AffineTransformation_MoveToLCS.md) | Преобразование совмещением глобальной системы координат с локальной |
|  | [Rotate](M_TFlex_Model_Model3D_Geometry_AffineTransformation_Rotate.md) | Вращение вокруг оси на заданный угол |
|  | [Scale](M_TFlex_Model_Model3D_Geometry_AffineTransformation_Scale.md) | Масштабирование по осям глобальной системы координат |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Transfer](M_TFlex_Model_Model3D_Geometry_AffineTransformation_Transfer.md) | Перемещение по вектору |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Multiply(AffineTransformation, AffineTransformation)](M_TFlex_Model_Model3D_Geometry_AffineTransformation_op_Multiply.md) |  |
  
#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
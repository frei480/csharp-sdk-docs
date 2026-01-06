

Руководство по T-FLEX CAD Open API

# LoftSphereVector - класс  
    
Класс для задания вектора в абсолютных или относительных сферических координатах

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3DLoftVectorDirection](T_TFlex_Model_Model3D_Loft_VectorDirection.md) TFlex.Model.Model3DLoftSphereVector

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class SphereVector : LoftVectorDirection
```
```vb
Public Class SphereVector
	Inherits LoftVectorDirection
```
```cpp
public ref class SphereVector : public LoftVectorDirection
```


Тип LoftSphereVector предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [LoftSphereVector(Parameter, Parameter, Parameter)](M_TFlex_Model_Model3D_Loft_SphereVector__ctor.md) | Конструктор для задания вектора в сферических координатах заданных в локальной системе координат |
|  | [LoftSphereVector(Parameter, Parameter, Parameter, LCS)](M_TFlex_Model_Model3D_Loft_SphereVector__ctor_1.md) | Конструктор для задания вектора в сферических координат заданных в локальной системе координат |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [LocalSystem](P_TFlex_Model_Model3D_Loft_SphereVector_LocalSystem.md) | Получить локальную систему координат |
|  | [Magnitude](P_TFlex_Model_Model3D_Loft_SphereVector_Magnitude.md) | Получить коэффициент вектора(Переопределяет VectorDirection.Magnitude) |
|  | [Phi](P_TFlex_Model_Model3D_Loft_SphereVector_Phi.md) | Возвращает координату Phi |
|  | [Theta](P_TFlex_Model_Model3D_Loft_SphereVector_Theta.md) | Возвращает координату Theta |
|  | [Type](P_TFlex_Model_Model3D_Loft_SphereVector_Type.md) | Получить тип векторного условия(Переопределяет [LoftVectorDirectionType](P_TFlex_Model_Model3D_Loft_VectorDirection_Type.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
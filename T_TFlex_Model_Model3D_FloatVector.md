

Руководство по T-FLEX CAD Open API

# FloatVector - структура  
    
Трехмерный вектор, элементы которого имеют тип float

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemValueType](https://learn.microsoft.com/dotnet/api/system.valuetype) TFlex.Model.Model3DFloatVector

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public struct FloatVector
```




Тип FloatVector предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [FloatVector(BaseDirection)](M_TFlex_Model_Model3D_FloatVector__ctor_1.md) | Конструктор, берущий координаты с вектора |
|  | [FloatVector(BasePoint3D)](M_TFlex_Model_Model3D_FloatVector__ctor_2.md) | Конструктор, берущий координаты с точки |
|  | [FloatVector(Single, Single, Single)](M_TFlex_Model_Model3D_FloatVector__ctor.md) | Конструктор, задающий начальные значения координат |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [data](P_TFlex_Model_Model3D_FloatVector_data.md) | Координанта |
|  | [x](P_TFlex_Model_Model3D_FloatVector_x.md) |  |
|  | [y](P_TFlex_Model_Model3D_FloatVector_y.md) | Координата y |
|  | [z](P_TFlex_Model_Model3D_FloatVector_z.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](M_TFlex_Model_Model3D_FloatVector_Equals.md) | Проверка равенства(Переопределяет [ValueTypeEquals(Object)](https://learn.microsoft.com/dotnet/api/system.valuetype.equals)) |
|  | [GetHashCode](M_TFlex_Model_Model3D_FloatVector_GetHashCode.md) | (Переопределяет [ValueTypeGetHashCode](https://learn.microsoft.com/dotnet/api/system.valuetype.gethashcode)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.valuetype.tostring) | Returns the fully qualified type name of this instance.(Унаследован от [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(FloatVector, FloatVector)](M_TFlex_Model_Model3D_FloatVector_op_Equality.md) | Проверка равенства |
|  | [(BaseDirection to FloatVector)](M_TFlex_Model_Model3D_FloatVector_op_Implicit.md) | Преобразование вектора |
|  | [(BasePoint3D to FloatVector)](M_TFlex_Model_Model3D_FloatVector_op_Implicit_1.md) | Преобразование точки |
|  | [Inequality(FloatVector, FloatVector)](M_TFlex_Model_Model3D_FloatVector_op_Inequality.md) | Проверка неравенства |
  
Доступ к элементам вектора возможен любым из способов: vec.x , vec.X , vec.data[0]

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
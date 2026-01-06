

Руководство по T-FLEX CAD Open API

# UnitConverter - класс  
    
Конвертер единиц измерения модели

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.GeometryUnitConverter

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class UnitConverter
```
```vb
Public NotInheritable Class UnitConverter
```
```cpp
public ref class UnitConverter sealed
```


Тип UnitConverter предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [UnitConverter](M_TFlex_Model_Model3D_Geometry_UnitConverter__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Scale](P_TFlex_Model_Model3D_Geometry_UnitConverter_Scale.md) | Коэффициент преобразования из единиц модели в метры |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FromMeter(BaseAxis)](M_TFlex_Model_Model3D_Geometry_UnitConverter_FromMeter_1.md) | Конвертировать координаты оси из метров в единицы модели |
|  | [FromMeter(BaseDirection)](M_TFlex_Model_Model3D_Geometry_UnitConverter_FromMeter_2.md) | Конвертировать координаты вектора направления из метров в единицы модели |
|  | [FromMeter(BasePlane)](M_TFlex_Model_Model3D_Geometry_UnitConverter_FromMeter_3.md) | Конвертировать координаты плоскости из метров в единицы модели |
|  | [FromMeter(BasePoint3D)](M_TFlex_Model_Model3D_Geometry_UnitConverter_FromMeter_4.md) | Конвертировать координаты точки из метров в единицы модели |
|  | [FromMeter(Double)](M_TFlex_Model_Model3D_Geometry_UnitConverter_FromMeter.md) | Конвертация из метров в единицы модели |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToMeter(BaseAxis)](M_TFlex_Model_Model3D_Geometry_UnitConverter_ToMeter_1.md) | Конвертировать координаты оси из единиц модели в метры |
|  | [ToMeter(BaseDirection)](M_TFlex_Model_Model3D_Geometry_UnitConverter_ToMeter_2.md) | Конвертировать координаты вектора направления из единиц модели в метры |
|  | [ToMeter(BasePlane)](M_TFlex_Model_Model3D_Geometry_UnitConverter_ToMeter_3.md) | Конвертировать координаты плоскости из единиц модели в метры |
|  | [ToMeter(BasePoint3D)](M_TFlex_Model_Model3D_Geometry_UnitConverter_ToMeter_4.md) | Конвертировать координаты точки из единиц модели в метры |
|  | [ToMeter(Double)](M_TFlex_Model_Model3D_Geometry_UnitConverter_ToMeter.md) | Конвертация из единиц модели в метры |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
В модели результирующая геометрия объектов хранится в метрах. Данный класс позволяет конвертировать геометрию в единицы модели и обратно

#### Ссылки

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
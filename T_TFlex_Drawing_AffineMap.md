

Руководство по T-FLEX CAD Open API

# AffineMap - класс  
  
---  
  
Класс двухмерного афинного преобразования

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.DrawingAffineMap

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class AffineMap : IDisposable
```
```vb
Public NotInheritable Class AffineMap
	Implements IDisposable
```
```cpp
public ref class AffineMap sealed : IDisposable
```


Тип AffineMap предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AffineMap](M_TFlex_Drawing_AffineMap__ctor.md) | Конструктор |
|  | [AffineMap(AffineMap)](M_TFlex_Drawing_AffineMap__ctor_3.md) | Конструктор |
|  | [AffineMap(Double, Double, Double)](M_TFlex_Drawing_AffineMap__ctor_1.md) | Конструктор |
|  | [AffineMap(Double, Double, Double, Double, Double, Double)](M_TFlex_Drawing_AffineMap__ctor_2.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Angle](P_TFlex_Drawing_AffineMap_Angle.md) | Угол афинного преобразования |
|  | [Scale](P_TFlex_Drawing_AffineMap_Scale.md) | Масштаб афинного преобразования |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ApplyToAngle](M_TFlex_Drawing_AffineMap_ApplyToAngle.md) | Применить афинное преобразование к углу |
|  | [Dispose](M_TFlex_Drawing_AffineMap_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Multiply](M_TFlex_Drawing_AffineMap_Multiply.md) | Умножить карту преобразования на другую карту |
|  | [ToLCS](M_TFlex_Drawing_AffineMap_ToLCS.md) | Отменить афинное преобразование |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToWCS](M_TFlex_Drawing_AffineMap_ToWCS.md) | Применить афинное преобразование |
  
#### Ссылки

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
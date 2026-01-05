

Руководство по T-FLEX CAD Open API

# Decoration - класс  
  
---  
  
Декорация

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3D.VisualDecoration [TFlex.Model.Model3D.VisualDecorationContainer](T_TFlex_Model_Model3D_Visual_DecorationContainer.md) [TFlex.Model.Model3D.VisualDecorationShape](T_TFlex_Model_Model3D_Visual_DecorationShape.md)

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public abstract class Decoration : IDisposable
```
```vb
Public MustInherit Class Decoration
	Implements IDisposable
```
```cpp
public ref class Decoration abstract : IDisposable
```


#### Значение поля

Декорации выводятся в 3D окнах поверх всех модельных объектов. 

Тип Decoration предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Decoration](M_TFlex_Model_Model3D_Visual_Decoration__ctor.md) | Инициализирует новый экземпляр класса Decoration |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Name](P_TFlex_Model_Model3D_Visual_Decoration_Name.md) | Имя декорации |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Decoration_Dispose.md) | Освобождает все ресурсы, используемые объектом Decoration |
|  | [Dispose(Boolean)](M_TFlex_Model_Model3D_Visual_Decoration_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом Decoration, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(Decoration, Decoration)](M_TFlex_Model_Model3D_Visual_Decoration_op_Equality.md) |  |
|  | [Inequality(Decoration, Decoration)](M_TFlex_Model_Model3D_Visual_Decoration_op_Inequality.md) |  |
  
Чтобы декорация стала изображаться, необходимо после создания добавить ее в [DecorationManager](T_TFlex_Model_Model3D_Visual_DecorationManager.md), диспетчер декораций или связать с [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md), манипулятором. 

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)
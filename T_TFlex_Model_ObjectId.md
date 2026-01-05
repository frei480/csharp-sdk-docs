

Руководство по T-FLEX CAD Open API

# ObjectId - класс  
  
---  
  
Класс идентификации объектов ModelObject

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelObjectId

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class ObjectId : IComparable, 
	ICloneable, IFormattable
```
```vb
Public NotInheritable Class ObjectId
	Implements IComparable, ICloneable, IFormattable
```
```cpp
public ref class ObjectId sealed : IComparable, 
	ICloneable, IFormattable
```


Тип ObjectId предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [IsValid](P_TFlex_Model_ObjectId_IsValid.md) | Является ли идентификатор корректным |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Clone](M_TFlex_Model_ObjectId_Clone.md) | Создает новый объект, являющийся копией текущего экземпляра. |
|  | [CompareTo](M_TFlex_Model_ObjectId_CompareTo.md) | Сравнивает текущий экземпляр с другим объектом того же типа и возвращает целое число, которое показывает, расположен ли текущий экземпляр перед, после или на той же позиции в порядке сортировки, что и другой объект. |
|  | [Create(UInt32)](M_TFlex_Model_ObjectId_Create.md) | Возвращает новый ObjectId, если oldID корректный. Иначе возвращает null. |
|  | [Create(UInt64)](M_TFlex_Model_ObjectId_Create_1.md) | Возвращает новый ObjectId, если idData корректный. Иначе возвращает null. |
|  | [Equals](M_TFlex_Model_ObjectId_Equals.md) | Определяет, равны ли два экземпляра объекта.(Переопределяет [ObjectEquals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\))) |
|  | [GetHashCode](M_TFlex_Model_ObjectId_GetHashCode.md) | Служит хэш-функцией по умолчанию.(Переопределяет [ObjectGetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Parse](M_TFlex_Model_ObjectId_Parse.md) | Распарсить строку в ObjectId. Выбросит исключение ArgumentException, если строка некорректна. |
|  | [ToString](M_TFlex_Model_ObjectId_ToString.md) | Возвращает строку, представляющую текущий объект.(Переопределяет [ObjectToString](https://learn.microsoft.com/dotnet/api/system.object.tostring)) |
|  | [ToString(String, IFormatProvider)](M_TFlex_Model_ObjectId_ToString_1.md) |  |
|  | [TryParse(String)](M_TFlex_Model_ObjectId_TryParse.md) | Распарсить строку в ObjectId. Вернет null, если строка некорректна. |
|  | [TryParse(String, ObjectId)](M_TFlex_Model_ObjectId_TryParse_1.md) | Распарсить строку в ObjectId. Вернет false, если строка некорректна. |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(ObjectId, ObjectId)](M_TFlex_Model_ObjectId_op_Equality.md) |  |
|  | [(ObjectId to UInt32)](M_TFlex_Model_ObjectId_op_Explicit.md) |  |
|  | [(ObjectId to UInt64)](M_TFlex_Model_ObjectId_op_Explicit_1.md) |  |
|  | [GreaterThan(ObjectId, ObjectId)](M_TFlex_Model_ObjectId_op_GreaterThan.md) |  |
|  | [GreaterThanOrEqual(ObjectId, ObjectId)](M_TFlex_Model_ObjectId_op_GreaterThanOrEqual.md) |  |
|  | [(UInt32 to ObjectId)](M_TFlex_Model_ObjectId_op_Implicit.md) |  |
|  | [(UInt64 to ObjectId)](M_TFlex_Model_ObjectId_op_Implicit_1.md) |  |
|  | [Inequality(ObjectId, ObjectId)](M_TFlex_Model_ObjectId_op_Inequality.md) |  |
|  | [LessThan(ObjectId, ObjectId)](M_TFlex_Model_ObjectId_op_LessThan.md) |  |
|  | [LessThanOrEqual(ObjectId, ObjectId)](M_TFlex_Model_ObjectId_op_LessThanOrEqual.md) |  |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
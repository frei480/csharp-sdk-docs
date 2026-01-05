

Руководство по T-FLEX CAD Open API

# Parameter - класс  
  
---  
  
Класс для хранения чиcловых переменных или констант

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelParameter

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class Parameter
```
```vb
Public Class Parameter
```
```cpp
public ref class Parameter
```


Тип Parameter предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Parameter(Double)](M_TFlex_Model_Parameter__ctor.md) | Конструктор для создания параметра, заданного вещественной константой |
|  | [Parameter(Int32)](M_TFlex_Model_Parameter__ctor_1.md) | Конструктор для создания параметра, заданного целочисленной константой |
|  | [Parameter(Variable)](M_TFlex_Model_Parameter__ctor_2.md) | Конструктор для создания параметра, заданного переменной |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [IntValue](P_TFlex_Model_Parameter_IntValue.md) | Константное значение в виде целого числа |
|  | [Value](P_TFlex_Model_Parameter_Value.md) | Константное значение в виде вещественного числа |
|  | [Variable](P_TFlex_Model_Parameter_Variable.md) | Ссылка на переменную |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Default](M_TFlex_Model_Parameter_Default.md) | Возвращает параметр с данными "из статуса" |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [(Double to Parameter)](M_TFlex_Model_Parameter_op_Implicit.md) | Оператор приведения к типу параметра |
|  | [(Int32 to Parameter)](M_TFlex_Model_Parameter_op_Implicit_1.md) | Оператор приведения к типу параметра |
|  | [(Variable to Parameter)](M_TFlex_Model_Parameter_op_Implicit_2.md) | Оператор приведения к типу параметра |
  
В отличие от класса хранения переменных и выражений данный класс не является экземпляром модели. Этот инструментальный класс используется для упрощения работы с параметрами объектов модели, которые могут задаваться как переменными, так и константами

#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)


Руководство по T-FLEX CAD Open API

# VariableParametric - класс  
  
---  
  
Класс определения свойств параметрических объектов, в котором положение копий задаётся набором явных функциональных зависимостей от номера копии

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3DParametric](T_TFlex_Model_Model3D_Parametric.md) TFlex.Model.Model3DVariableParametric

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class VariableParametric : Parametric
```
```vb
Public NotInheritable Class VariableParametric
	Inherits Parametric
```
```cpp
public ref class VariableParametric sealed : public Parametric
```


Тип VariableParametric предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AxisX](P_TFlex_Model_Model3D_VariableParametric_AxisX.md) | Функции, задающие ориентацию оси X системы координат копии |
|  | [AxisY](P_TFlex_Model_Model3D_VariableParametric_AxisY.md) | Функции, задающие ориентацию оси Y системы координат копии |
|  | [AxisZ](P_TFlex_Model_Model3D_VariableParametric_AxisZ.md) | Функции, задающие ориентацию оси Z системы координат копии |
|  | [Number](P_TFlex_Model_Model3D_Parametric_Number.md) | Переменная номера копии(Унаследован от [Parametric](T_TFlex_Model_Model3D_Parametric.md)) |
|  | [Origin](P_TFlex_Model_Model3D_VariableParametric_Origin.md) | Функции, задающие положение системы координат копии |
|  | [Quantity](P_TFlex_Model_Model3D_Parametric_Quantity.md) | Количество копий(Унаследован от [Parametric](T_TFlex_Model_Model3D_Parametric.md)) |
|  | [SourceLCS](P_TFlex_Model_Model3D_Parametric_SourceLCS.md) | Исходная система координат(Унаследован от [Parametric](T_TFlex_Model_Model3D_Parametric.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Положение копии задаётся локальной системой координат. Нулевая точка и направление осей такой системы координат определяются функциями. К каждой копии применяется преобразование из системы координат для первой копии или ЛСК (если задана) в систему координат для текущей копии. Таким образом, первый элемент массива остаётся на месте. Если для системы координат функциональные зависимости не заданы, то, по умолчанию, она совпадает с глобальной системой координат и трансформация не выполняется.

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
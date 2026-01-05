

Руководство по T-FLEX CAD Open API

# EdgeBlendingVariableBlendAttribute - класс  
  
---  
  
Класс для задания свойств с переменным радиусом скругления

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3DEdgeBlendingAttribute](T_TFlex_Model_Model3D_EdgeBlending_Attribute.md) TFlex.Model.Model3DEdgeBlendingVariableBlendAttribute

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class VariableBlendAttribute : EdgeBlendingAttribute
```
```vb
Public Class VariableBlendAttribute
	Inherits EdgeBlendingAttribute
```
```cpp
public ref class VariableBlendAttribute : public EdgeBlendingAttribute
```


Тип EdgeBlendingVariableBlendAttribute предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [EdgeBlendingVariableBlendAttribute(Parameter, Parameter)](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute__ctor_1.md) | Конструктор |
|  | [EdgeBlendingVariableBlendAttribute(EdgeBlendingPositionData, EdgeBlendingPositionData)](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute__ctor.md) | Конструктор |
|  | [EdgeBlendingVariableBlendAttribute(Parameter, Parameter, Parameter)](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute__ctor_2.md) | Конструктор |
|  | [EdgeBlendingVariableBlendAttribute(Parameter, Parameter, Parameter, Parameter, Parameter)](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute__ctor_3.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [PositionCount](P_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_PositionCount.md) | Число позиций |
|  | [SetbackEnd](P_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_SetbackEnd.md) | Отступ от конца ребра |
|  | [SetbackStart](P_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_SetbackStart.md) | Отступ от начала ребра |
|  | [Type](P_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_Type.md) | Тип свойства(Переопределяет [EdgeBlendingAttributeType](P_TFlex_Model_Model3D_EdgeBlending_Attribute_Type.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddPosition](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_AddPosition.md) | Добавить позицию |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetPosition](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_GetPosition.md) | Добавить позицию |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [RemoveAllPositions](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_RemoveAllPositions.md) | Добавить позицию |
|  | [RemovePosition](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_RemovePosition.md) | Добавить позицию |
|  | [SetPosition](M_TFlex_Model_Model3D_EdgeBlending_VariableBlendAttribute_SetPosition.md) | Установить данные позиции |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
VariableBlendAttribute является временным объектом используемым для облегчения задания свойств операции сглаживания

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
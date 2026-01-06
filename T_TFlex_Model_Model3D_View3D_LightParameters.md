

Руководство по T-FLEX CAD Open API

# View3DLightParameters - класс  
    
Параметры освещения 3D вида

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Model3DView3DLightParameters

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class LightParameters : ICloneable
```
```vb
Public Class LightParameters
	Implements ICloneable
```
```cpp
public ref class LightParameters : ICloneable
```


Тип View3DLightParameters предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [View3DLightParameters](M_TFlex_Model_Model3D_View3D_LightParameters__ctor.md) | Конструктор по умолчанию |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [DirectionalLight](P_TFlex_Model_Model3D_View3D_LightParameters_DirectionalLight.md) | Направленный источник света с заданным индексом |
|  | [DirectionalLights](P_TFlex_Model_Model3D_View3D_LightParameters_DirectionalLights.md) |  |
|  | [EnvironmentLight](P_TFlex_Model_Model3D_View3D_LightParameters_EnvironmentLight.md) | Параметры рассеянного освещения |
|  | [NumDirectionalLights](P_TFlex_Model_Model3D_View3D_LightParameters_NumDirectionalLights.md) | Количество направленных источников света |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDirectionalLight](M_TFlex_Model_Model3D_View3D_LightParameters_AddDirectionalLight.md) | Добавляет новый источник света |
|  | [Clone](M_TFlex_Model_Model3D_View3D_LightParameters_Clone.md) | Возвращает копию объекта |
|  | [DeleteDirectionalLight](M_TFlex_Model_Model3D_View3D_LightParameters_DeleteDirectionalLight.md) | Удаляет источник света с заданным индексом |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(View3DLightParameters, View3DLightParameters)](M_TFlex_Model_Model3D_View3D_LightParameters_op_Equality.md) |  |
|  | [Inequality(View3DLightParameters, View3DLightParameters)](M_TFlex_Model_Model3D_View3D_LightParameters_op_Inequality.md) |  |
  
Освещение складывается из рассеянного освещения и направленных источников света. Наличие направленных источников необязательно. Их максимальное число зависит от используемой видеокарты и драйверов OpenGL.

#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
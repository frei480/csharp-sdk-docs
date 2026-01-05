

Руководство по T-FLEX CAD Open API

# Object3DSetGeomReference(Int32, Object3DGeomReference) - метод  
  
---  
  
Установить ссылку на родительский объект по ключу

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual void SetGeomReference(
	int id,
	Object3DGeomReference reference
)
```
```vb
Public Overridable Sub SetGeomReference ( 
	id As Integer,
	reference As Object3DGeomReference
)
```
```cpp
public:
virtual void SetGeomReference(
	int id, 
	Object3DGeomReference^ reference
)
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор ключа, по которому в контейнере ссылок хранится объект
reference [Object3DGeomReference](T_TFlex_Model_Model3D_Object3D_GeomReference.md)
    Ссылка на родительский объект

#### Ссылки

[Object3D - ](T_TFlex_Model_Model3D_Object3D.md)

[SetGeomReference - перегрузка](Overload_TFlex_Model_Model3D_Object3D_SetGeomReference.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
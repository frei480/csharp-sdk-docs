

Руководство по T-FLEX CAD Open API

# Object3DGetGeomReference(Int32, ModelObjectArrayIndices) - метод  
    
Получить ссылку на родительский объект по ключу и индексу

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public virtual Geometry GetGeomReference(
	int id,
	ModelObjectArrayIndices indices
)
```




#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор ключа, по которому в контейнере ссылок хранится объект
indices [ModelObjectArrayIndices](T_TFlex_Model_ModelObject_ArrayIndices.md)
    Координаты элемента

#### Возвращаемое значение

[Geometry](T_TFlex_Model_Model3D_Geometry_Geometry.md)

Используется для организации массивов. Поскольку геометрические данные связаны с родительской операцией, то саму родительскую операцию также можно получить по такому же ключу через функции [GetReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetReference.md) />

#### Ссылки

[Object3D - ](T_TFlex_Model_Model3D_Object3D.md)

[GetGeomReference - перегрузка](Overload_TFlex_Model_Model3D_Object3D_GetGeomReference.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
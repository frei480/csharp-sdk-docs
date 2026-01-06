

Руководство по T-FLEX CAD Open API

# FaceFaceBlendGenerator - конструктор  
    
Конструктор для задания базовых объектов сглаживания

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FaceFaceBlendGenerator(
	ProxyObject3D object,
	Body body,
	bool leftSense,
	bool rightSense,
	TFBlendMode bm,
	TFCutMode cm,
	TFPlaneOrientation po
)
```




#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
body [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Тело на котором строится сглаживание
leftSense [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр ориентации левой стенки
rightSense [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр ориентации правой стенки
bm [TFBlendMode](T_TFlex_Model_Model3D_Geometry_TFBlendMode.md)
    Режим сглаживания
cm [TFCutMode](T_TFlex_Model_Model3D_Geometry_TFCutMode.md)
    Режим обрезки результата
po [TFPlaneOrientation](T_TFlex_Model_Model3D_Geometry_TFPlaneOrientation.md)
    Режим ориентации плоскости сечения сглажиавния

3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[FaceFaceBlendGenerator - ](T_TFlex_Model_Model3D_Geometry_FaceFaceBlendGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
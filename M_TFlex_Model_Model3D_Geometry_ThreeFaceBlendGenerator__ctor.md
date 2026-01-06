

Руководство по T-FLEX CAD Open API

# ThreeFaceBlendGenerator - конструктор  
    
Конструктор для задания базовых объектов сглаживания

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ThreeFaceBlendGenerator(
	ProxyObject3D object,
	Body body,
	SenseOfFace leftSense,
	SenseOfFace centerSense,
	SenseOfFace rightSense,
	bool propagateBlend
)
```




#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
body [Body](T_TFlex_Model_Model3D_Geometry_Body.md)
    Тело на котором строится сглаживание
leftSense [SenseOfFace](T_TFlex_Model_Model3D_Geometry_SenseOfFace.md)
    Параметр ориентации левой стенки
centerSense [SenseOfFace](T_TFlex_Model_Model3D_Geometry_SenseOfFace.md)
    Параметр ориентации центральной стенки
rightSense [SenseOfFace](T_TFlex_Model_Model3D_Geometry_SenseOfFace.md)
    Параметр ориентации правой стенки
propagateBlend [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Продолжать ли сглаживание на гладкую последовательность граней

3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[ThreeFaceBlendGenerator - ](T_TFlex_Model_Model3D_Geometry_ThreeFaceBlendGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
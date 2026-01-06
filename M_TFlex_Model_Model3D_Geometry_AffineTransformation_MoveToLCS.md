

Руководство по T-FLEX CAD Open API

# AffineTransformationMoveToLCS - метод  
    
Преобразование совмещением глобальной системы координат с локальной

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static AffineTransformation MoveToLCS(
	BasePoint3D origin,
	BaseDirection zaxis,
	BaseDirection xaxis
)
```
```vb
Public Shared Function MoveToLCS ( 
	origin As BasePoint3D,
	zaxis As BaseDirection,
	xaxis As BaseDirection
) As AffineTransformation
```
```cpp
public:
static AffineTransformation^ MoveToLCS(
	BasePoint3D^ origin, 
	BaseDirection^ zaxis, 
	BaseDirection^ xaxis
)
```


#### Параметры

origin [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    Начало локальной системы координат
zaxis [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Ось Z локальной системы координат
xaxis [BaseDirection](T_TFlex_Model_Model3D_Geometry_BaseDirection.md)
    Ось X локальной системы координат

#### Возвращаемое значение

[AffineTransformation](T_TFlex_Model_Model3D_Geometry_AffineTransformation.md)

#### Ссылки

[AffineTransformation - ](T_TFlex_Model_Model3D_Geometry_AffineTransformation.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)


Руководство по T-FLEX CAD Open API

# BaseSurfaceDerivative - метод  
  
---  
  
Вычислить производные в точке на поверхности по параметрам

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Direction[] Derivative(
	UV uv,
	uint uderivs,
	uint vderivs
)
```
```vb
Public Function Derivative ( 
	uv As UV,
	uderivs As UInteger,
	vderivs As UInteger
) As Direction()
```
```cpp
public:
array<Direction^>^ Derivative(
	UV uv, 
	unsigned int uderivs, 
	unsigned int vderivs
)
```


#### Параметры

uv [UV](T_TFlex_Model_Model3D_Geometry_UV.md)
    Параметры на поверхности
uderivs [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Максимальный порядок производной по U
vderivs [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Максимальный порядок производной по V

#### Возвращаемое значение

[Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)

Производные возвращаются в следующем порядке: i-ая производная ( i <= 'uderivs' ) по u и j-ая производная ( j <= 'vderivs' ) по v хранится по индексу = i + ( 'uderivs' + 1 ) ^ j ). Например, если 'uderivs' == 2 и 'vderivs' == 3, тогда массив из 12 векторов выглядит следующим образом : p(u,v) p(u,v) p(u,v) u uu Затем: p(u,v) p(u,v) p(u,v) v uv uuv Затем: p(u,v) p(u,v) p(u,v) vv uvv uuvv Затем: p(u,v) p(u,v) p(u,v) vvv uvvv uuvvv Здесь запись : p(u,v) uvv \- означает первую производную по u и вторую производную по V 

#### Ссылки

[BaseSurface - ](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
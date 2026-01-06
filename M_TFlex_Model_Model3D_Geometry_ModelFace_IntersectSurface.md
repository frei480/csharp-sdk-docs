

Руководство по T-FLEX CAD Open API

# ModelFaceIntersectSurface - метод  
    
Найти пересечение грани с другой поверхностью

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public IntersectSurfaceData IntersectSurface(
	BaseSurface surface,
	bool havebox,
	BaseBox box,
	bool haveuvbox1,
	UVBox uvbox1,
	bool haveuvbox2,
	UVBox uvbox2,
	bool havepoint,
	BasePoint3D point
)
```
```vb
Public Function IntersectSurface ( 
	surface As BaseSurface,
	havebox As Boolean,
	box As BaseBox,
	haveuvbox1 As Boolean,
	uvbox1 As UVBox,
	haveuvbox2 As Boolean,
	uvbox2 As UVBox,
	havepoint As Boolean,
	point As BasePoint3D
) As IntersectSurfaceData
```
```cpp
public:
IntersectSurfaceData^ IntersectSurface(
	BaseSurface^ surface, 
	bool havebox, 
	BaseBox^ box, 
	bool haveuvbox1, 
	UVBox^ uvbox1, 
	bool haveuvbox2, 
	UVBox^ uvbox2, 
	bool havepoint, 
	BasePoint3D^ point
)
```


#### Параметры

surface [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)
    Поверхность, с которой ищется пересечение
havebox [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать область поиска пересечений
box [BaseBox](T_TFlex_Model_Model3D_Geometry_BaseBox.md)
    Область поиска пересечений
haveuvbox1 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать параметрическую область поиска пересечений для первой поверхности
uvbox1 [UVBox](T_TFlex_Model_Model3D_Geometry_UVBox.md)
    Параметрическая область поиска пересечений для первой поверхности
haveuvbox2 [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать параметрическую область поиска пересечений для второй поверхности
uvbox2 [UVBox](T_TFlex_Model_Model3D_Geometry_UVBox.md)
    Параметрическая область поиска пересечений для второй поверхности
havepoint [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать точку для отбора одной из нескольких веток пересечения, на которой лежит точка
point [BasePoint3D](T_TFlex_Model_Model3D_Geometry_BasePoint3D.md)
    Точка для отбора одной из нескольких веток пересечения, на которой лежит точка

#### Возвращаемое значение

[IntersectSurfaceData](T_TFlex_Model_Model3D_Geometry_IntersectSurfaceData.md)

#### Ссылки

[ModelFace - ](T_TFlex_Model_Model3D_Geometry_ModelFace.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
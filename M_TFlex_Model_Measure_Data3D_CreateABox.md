

Руководство по T-FLEX CAD Open API

# Data3DCreateABox - метод  
  **Пространство имён:** [TFlex.Model.Measure](N_TFlex_Model_Measure.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Data CreateABox(
	ulong id,
	string name,
	Point3D origin,
	Direction axis,
	Direction ref_dir,
	Point3D size
)
```
```vb
Public Shared Function CreateABox ( 
	id As ULong,
	name As String,
	origin As Point3D,
	axis As Direction,
	ref_dir As Direction,
	size As Point3D
) As Data
```
```cpp
public:
static Data^ CreateABox(
	unsigned long long id, 
	String^ name, 
	Point3D^ origin, 
	Direction^ axis, 
	Direction^ ref_dir, 
	Point3D^ size
)
```


#### Параметры

id [UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    
origin [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    
axis [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
ref_dir [Direction](T_TFlex_Model_Model3D_Geometry_Direction.md)
    
size [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    

#### Возвращаемое значение

[Data](T_TFlex_Model_Measure_Data.md)

#### Ссылки

[Data3D - ](T_TFlex_Model_Measure_Data3D.md)

[TFlex.Model.Measure - пространство имён](N_TFlex_Model_Measure.md)
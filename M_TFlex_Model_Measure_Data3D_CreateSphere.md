

Руководство по T-FLEX CAD Open API

# Data3DCreateSphere - метод  
  
---  
**Пространство имён:** [TFlex.Model.Measure](N_TFlex_Model_Measure.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Data CreateSphere(
	ulong id,
	string name,
	Point3D origin,
	double radius
)
```
```vb
Public Shared Function CreateSphere ( 
	id As ULong,
	name As String,
	origin As Point3D,
	radius As Double
) As Data
```
```cpp
public:
static Data^ CreateSphere(
	unsigned long long id, 
	String^ name, 
	Point3D^ origin, 
	double radius
)
```


#### Параметры

id [UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    
origin [Point3D](T_TFlex_Model_Model3D_Geometry_Point3D.md)
    
radius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Data](T_TFlex_Model_Measure_Data.md)

#### Ссылки

[Data3D - ](T_TFlex_Model_Measure_Data3D.md)

[TFlex.Model.Measure - пространство имён](N_TFlex_Model_Measure.md)
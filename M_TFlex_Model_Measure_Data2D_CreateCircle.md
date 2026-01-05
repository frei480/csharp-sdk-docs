

Руководство по T-FLEX CAD Open API

# Data2DCreateCircle - метод  
  
---  
**Пространство имён:** [TFlex.Model.Measure](N_TFlex_Model_Measure.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Data CreateCircle(
	ulong id,
	string name,
	Page page,
	Point origin,
	double radius
)
```
```vb
Public Shared Function CreateCircle ( 
	id As ULong,
	name As String,
	page As Page,
	origin As Point,
	radius As Double
) As Data
```
```cpp
public:
static Data^ CreateCircle(
	unsigned long long id, 
	String^ name, 
	Page^ page, 
	Point origin, 
	double radius
)
```


#### Параметры

id [UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    
page [Page](T_TFlex_Model_Page.md)
    
origin [Point](T_TFlex_Drawing_Point.md)
    
radius [Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Data](T_TFlex_Model_Measure_Data.md)

#### Ссылки

[Data2D - ](T_TFlex_Model_Measure_Data2D.md)

[TFlex.Model.Measure - пространство имён](N_TFlex_Model_Measure.md)


Руководство по T-FLEX CAD Open API

# Data2DCreateLabel - метод  
  
---  
**Пространство имён:** [TFlex.Model.Measure](N_TFlex_Model_Measure.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Data CreateLabel(
	ulong id,
	string name,
	Page page,
	string text,
	Point point,
	Point delta
)
```
```vb
Public Shared Function CreateLabel ( 
	id As ULong,
	name As String,
	page As Page,
	text As String,
	point As Point,
	delta As Point
) As Data
```
```cpp
public:
static Data^ CreateLabel(
	unsigned long long id, 
	String^ name, 
	Page^ page, 
	String^ text, 
	Point point, 
	Point delta
)
```


#### Параметры

id [UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    
page [Page](T_TFlex_Model_Page.md)
    
text [String](https://learn.microsoft.com/dotnet/api/system.string)
    
point [Point](T_TFlex_Drawing_Point.md)
    
delta [Point](T_TFlex_Drawing_Point.md)
    

#### Возвращаемое значение

[Data](T_TFlex_Model_Measure_Data.md)

#### Ссылки

[Data2D - ](T_TFlex_Model_Measure_Data2D.md)

[TFlex.Model.Measure - пространство имён](N_TFlex_Model_Measure.md)
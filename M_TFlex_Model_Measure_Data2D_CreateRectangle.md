

Руководство по T-FLEX CAD Open API

# Data2DCreateRectangle - метод  
  **Пространство имён:** [TFlex.Model.Measure](N_TFlex_Model_Measure.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Data CreateRectangle(
	ulong id,
	string name,
	Page page,
	Rectangle rect
)
```
```vb
Public Shared Function CreateRectangle ( 
	id As ULong,
	name As String,
	page As Page,
	rect As Rectangle
) As Data
```
```cpp
public:
static Data^ CreateRectangle(
	unsigned long long id, 
	String^ name, 
	Page^ page, 
	Rectangle rect
)
```


#### Параметры

id [UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    
page [Page](T_TFlex_Model_Page.md)
    
rect [Rectangle](T_TFlex_Drawing_Rectangle.md)
    

#### Возвращаемое значение

[Data](T_TFlex_Model_Measure_Data.md)

#### Ссылки

[Data2D - ](T_TFlex_Model_Measure_Data2D.md)

[TFlex.Model.Measure - пространство имён](N_TFlex_Model_Measure.md)
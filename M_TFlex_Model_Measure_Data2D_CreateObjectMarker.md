

Руководство по T-FLEX CAD Open API

# Data2DCreateObjectMarker(UInt64, String, Page, ListObjectId) - метод  
  
---  
**Пространство имён:** [TFlex.Model.Measure](N_TFlex_Model_Measure.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Data CreateObjectMarker(
	ulong id,
	string name,
	Page page,
	List<ObjectId> objectIDs
)
```
```vb
Public Shared Function CreateObjectMarker ( 
	id As ULong,
	name As String,
	page As Page,
	objectIDs As List(Of ObjectId)
) As Data
```
```cpp
public:
static Data^ CreateObjectMarker(
	unsigned long long id, 
	String^ name, 
	Page^ page, 
	List<ObjectId^>^ objectIDs
)
```


#### Параметры

id [UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    
page [Page](T_TFlex_Model_Page.md)
    
objectIDs [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[ObjectId](T_TFlex_Model_ObjectId.md)
    

#### Возвращаемое значение

[Data](T_TFlex_Model_Measure_Data.md)

#### Ссылки

[Data2D - ](T_TFlex_Model_Measure_Data2D.md)

[CreateObjectMarker - перегрузка](Overload_TFlex_Model_Measure_Data2D_CreateObjectMarker.md)

[TFlex.Model.Measure - пространство имён](N_TFlex_Model_Measure.md)
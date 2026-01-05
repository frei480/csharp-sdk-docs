

Руководство по T-FLEX CAD Open API

# ProductStructureReportSupportTryCopyAllReportRowElementsToAssembly - метод  
  
---  
**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static bool TryCopyAllReportRowElementsToAssembly(
	IntPtr docHandle,
	ulong psID,
	Guid generId,
	string psReportId,
	bool silent
)
```
```vb
Public Shared Function TryCopyAllReportRowElementsToAssembly ( 
	docHandle As IntPtr,
	psID As ULong,
	generId As Guid,
	psReportId As String,
	silent As Boolean
) As Boolean
```
```cpp
public:
static bool TryCopyAllReportRowElementsToAssembly(
	IntPtr docHandle, 
	unsigned long long psID, 
	Guid generId, 
	String^ psReportId, 
	bool silent
)
```


#### Параметры

docHandle [IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)
    
psID [UInt64](https://learn.microsoft.com/dotnet/api/system.uint64)
    
generId [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    
psReportId [String](https://learn.microsoft.com/dotnet/api/system.string)
    
silent [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ProductStructureReportSupport - ](T_TFlex_Model_ProductStructureReportSupport.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
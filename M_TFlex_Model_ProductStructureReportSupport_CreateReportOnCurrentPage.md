

Руководство по T-FLEX CAD Open API

# ProductStructureReportSupportCreateReportOnCurrentPage - метод  
  
---  
**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static bool CreateReportOnCurrentPage(
	Document document,
	Document templateDocument,
	string textName,
	bool searchKnots,
	bool quietMode,
	ParagraphTextTextRectangle? prevRect,
	ref bool isCommandStarted,
	ref bool userCanceled
)
```
```vb
Public Shared Function CreateReportOnCurrentPage ( 
	document As Document,
	templateDocument As Document,
	textName As String,
	searchKnots As Boolean,
	quietMode As Boolean,
	prevRect As ParagraphTextTextRectangle?,
	ByRef isCommandStarted As Boolean,
	ByRef userCanceled As Boolean
) As Boolean
```
```cpp
public:
static bool CreateReportOnCurrentPage(
	Document^ document, 
	Document^ templateDocument, 
	String^ textName, 
	bool searchKnots, 
	bool quietMode, 
	Nullable<ParagraphTextTextRectangle> prevRect, 
	bool% isCommandStarted, 
	bool% userCanceled
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    
templateDocument [Document](T_TFlex_Model_Document.md)
    
textName [String](https://learn.microsoft.com/dotnet/api/system.string)
    
searchKnots [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
quietMode [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
prevRect [Nullable](https://learn.microsoft.com/dotnet/api/system.nullable-1)[ParagraphTextTextRectangle](T_TFlex_Model_Model2D_ParagraphText_TextRectangle.md)
    
isCommandStarted [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
userCanceled [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ProductStructureReportSupport - ](T_TFlex_Model_ProductStructureReportSupport.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
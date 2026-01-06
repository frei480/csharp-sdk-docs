

Руководство по T-FLEX CAD Open API

# ConductorConnect - метод  
  **Пространство имён:** [TFlex.Model.Model3D.ConductorModel](N_TFlex_Model_Model3D_ConductorModel.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Conductor Connect(
	Segment segment,
	double paramByLength,
	TerminalPoint last,
	SegmentCurveType type,
	string sleeveFileName,
	bool firstOrLastPoint
)
```
```vb
Public Function Connect ( 
	segment As Segment,
	paramByLength As Double,
	last As TerminalPoint,
	type As SegmentCurveType,
	sleeveFileName As String,
	firstOrLastPoint As Boolean
) As Conductor
```
```cpp
public:
Conductor^ Connect(
	Segment^ segment, 
	double paramByLength, 
	TerminalPoint^ last, 
	SegmentCurveType type, 
	String^ sleeveFileName, 
	bool firstOrLastPoint
)
```


#### Параметры

segment [Segment](T_TFlex_Model_Model3D_ConductorModel_Segment.md)
    
paramByLength [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
last [TerminalPoint](T_TFlex_Model_Model3D_ConductorModel_TerminalPoint.md)
    
type [SegmentCurveType](T_TFlex_Model_Model3D_ConductorModel_Segment_CurveType.md)
    
sleeveFileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    
firstOrLastPoint [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[Conductor](T_TFlex_Model_Model3D_ConductorModel_Conductor.md)

#### Ссылки

[Conductor - ](T_TFlex_Model_Model3D_ConductorModel_Conductor.md)

[TFlex.Model.Model3D.ConductorModel - пространство имён](N_TFlex_Model_Model3D_ConductorModel.md)
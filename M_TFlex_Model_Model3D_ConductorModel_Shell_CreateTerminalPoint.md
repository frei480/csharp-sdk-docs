

Руководство по T-FLEX CAD Open API

# ShellCreateTerminalPoint - метод  
  **Пространство имён:** [TFlex.Model.Model3D.ConductorModel](N_TFlex_Model_Model3D_ConductorModel.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public TerminalPoint CreateTerminalPoint(
	Segment segment,
	bool sense,
	Parameter offset
)
```
```vb
Public Function CreateTerminalPoint ( 
	segment As Segment,
	sense As Boolean,
	offset As Parameter
) As TerminalPoint
```
```cpp
public:
TerminalPoint^ CreateTerminalPoint(
	Segment^ segment, 
	bool sense, 
	Parameter^ offset
)
```


#### Параметры

segment [Segment](T_TFlex_Model_Model3D_ConductorModel_Segment.md)
    
sense [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
offset [Parameter](T_TFlex_Model_Parameter.md)
    

#### Возвращаемое значение

[TerminalPoint](T_TFlex_Model_Model3D_ConductorModel_TerminalPoint.md)

#### Ссылки

[Shell - ](T_TFlex_Model_Model3D_ConductorModel_Shell.md)

[TFlex.Model.Model3D.ConductorModel - пространство имён](N_TFlex_Model_Model3D_ConductorModel.md)


Руководство по T-FLEX CAD Open API

# PopupManagerShowSelectToleranceWindow - метод  
  **Пространство имён:** [TFlex.ControlService](N_TFlex_ControlService.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public static bool ShowSelectToleranceWindow(
	double nominal,
	Unit unit,
	out ToleranceProperties properties
)
```
```vb
Public Shared Function ShowSelectToleranceWindow ( 
	nominal As Double,
	unit As Unit,
	<OutAttribute> ByRef properties As ToleranceProperties
) As Boolean
```
```cpp
public:
static bool ShowSelectToleranceWindow(
	double nominal, 
	Unit^ unit, 
	[OutAttribute] ToleranceProperties^% properties
)
```


#### Параметры

nominal [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
unit [Unit](T_TFlex_Model_Units_Unit.md)
    
properties [ToleranceProperties](T_TFlex_ControlService_ToleranceProperties.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[PopupManager - ](T_TFlex_ControlService_PopupManager.md)

[TFlex.ControlService - пространство имён](N_TFlex_ControlService.md)
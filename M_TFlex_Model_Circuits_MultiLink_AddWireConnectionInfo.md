

Руководство по T-FLEX CAD Open API

# MultiLinkAddWireConnectionInfo - метод  
  **Пространство имён:** [TFlex.Model.Circuits](N_TFlex_Model_Circuits.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public override WireConnectionInfo AddWireConnectionInfo(
	Element wire,
	ModelObject start,
	ModelObject end
)
```
```vb
Public Overrides Function AddWireConnectionInfo ( 
	wire As Element,
	start As ModelObject,
	end As ModelObject
) As WireConnectionInfo
```
```cpp
public:
virtual WireConnectionInfo^ AddWireConnectionInfo(
	Element^ wire, 
	ModelObject^ start, 
	ModelObject^ end
) override
```


#### Параметры

wire [Element](T_TFlex_Model_Structure_Element.md)
    
start [ModelObject](T_TFlex_Model_ModelObject.md)
    
end [ModelObject](T_TFlex_Model_ModelObject.md)
    

#### Возвращаемое значение

[WireConnectionInfo](T_TFlex_Model_Circuits_WireConnectionInfo.md)

#### Ссылки

[MultiLink - ](T_TFlex_Model_Circuits_MultiLink.md)

[TFlex.Model.Circuits - пространство имён](N_TFlex_Model_Circuits.md)
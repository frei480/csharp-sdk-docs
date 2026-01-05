

Руководство по T-FLEX CAD Open API

# ExternalOperation - конструктор  
  
---  
  
Конструктор для создания внешней операции

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ExternalOperation(
	ProxyOperation proxy,
	Document document,
	Plugin application
)
```
```vb
Public Sub New ( 
	proxy As ProxyOperation,
	document As Document,
	application As Plugin
)
```
```cpp
public:
ExternalOperation(
	ProxyOperation^ proxy, 
	Document^ document, 
	Plugin^ application
)
```


#### Параметры

proxy [ProxyOperation](T_TFlex_Model_Model3D_ProxyOperation.md)
    3D операция внешнего приложения
document [Document](T_TFlex_Model_Document.md)
    Документ, в котором создаётся новый объект
application [Plugin](T_TFlex_Plugin.md)
    Плагин

#### Ссылки

[ExternalOperation - ](T_TFlex_Model_Model3D_ExternalOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
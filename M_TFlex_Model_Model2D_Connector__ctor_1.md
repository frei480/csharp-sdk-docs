

Руководство по T-FLEX CAD Open API

# Connector(Document, Fragment, String) - конструктор  
  
---  
  
Конструктор, создающий ссылочный коннектор фрагмента

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Connector(
	Document document,
	Fragment fragment,
	string connectorComment
)
```
```vb
Public Sub New ( 
	document As Document,
	fragment As Fragment,
	connectorComment As String
)
```
```cpp
public:
Connector(
	Document^ document, 
	Fragment^ fragment, 
	String^ connectorComment
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ объекта
fragment [Fragment](T_TFlex_Model_Model2D_Fragment.md)
    Фрагмент, содержащий коннектор, который требуется перевести в сборку
connectorComment [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя коннектора в документе фрагмента, который требуется перевести в сборку

#### Ссылки

[Connector - ](T_TFlex_Model_Model2D_Connector.md)

[Connector - перегрузка](Overload_TFlex_Model_Model2D_Connector__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
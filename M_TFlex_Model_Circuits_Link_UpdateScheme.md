

Руководство по T-FLEX CAD Open API

# LinkUpdateScheme - метод  
  **Пространство имён:** [TFlex.Model.Circuits](N_TFlex_Model_Circuits.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static void UpdateScheme(
	Document targetDocument,
	Dictionary<LinkBase, LinkBase> links,
	Dictionary<ModelObject, ModelObject> connectors,
	Dictionary<Page, Page> pages
)
```
```vb
Public Shared Sub UpdateScheme ( 
	targetDocument As Document,
	links As Dictionary(Of LinkBase, LinkBase),
	connectors As Dictionary(Of ModelObject, ModelObject),
	pages As Dictionary(Of Page, Page)
)
```
```cpp
public:
static void UpdateScheme(
	Document^ targetDocument, 
	Dictionary<LinkBase^, LinkBase^>^ links, 
	Dictionary<ModelObject^, ModelObject^>^ connectors, 
	Dictionary<Page^, Page^>^ pages
)
```


#### Параметры

targetDocument [Document](T_TFlex_Model_Document.md)
    
links [Dictionary](https://learn.microsoft.com/dotnet/api/system.collections.generic.dictionary-2)[LinkBase](T_TFlex_Model_Circuits_LinkBase.md), [LinkBase](T_TFlex_Model_Circuits_LinkBase.md)
    
connectors [Dictionary](https://learn.microsoft.com/dotnet/api/system.collections.generic.dictionary-2)[ModelObject](T_TFlex_Model_ModelObject.md), [ModelObject](T_TFlex_Model_ModelObject.md)
    
pages [Dictionary](https://learn.microsoft.com/dotnet/api/system.collections.generic.dictionary-2)[Page](T_TFlex_Model_Page.md), [Page](T_TFlex_Model_Page.md)
    

#### Ссылки

[Link - ](T_TFlex_Model_Circuits_Link.md)

[TFlex.Model.Circuits - пространство имён](N_TFlex_Model_Circuits.md)
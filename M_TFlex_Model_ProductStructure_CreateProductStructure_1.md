

Руководство по T-FLEX CAD Open API

# ProductStructureCreateProductStructure(Document, FileLink) - метод  
  
---  
  
Создать новую структуру изделия

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static ProductStructure CreateProductStructure(
	Document doc,
	FileLink schemeFileLink
)
```
```vb
Public Shared Function CreateProductStructure ( 
	doc As Document,
	schemeFileLink As FileLink
) As ProductStructure
```
```cpp
public:
static ProductStructure^ CreateProductStructure(
	Document^ doc, 
	FileLink^ schemeFileLink
)
```


#### Параметры

doc [Document](T_TFlex_Model_Document.md)
    Документ, в котором создаётся новая структура
schemeFileLink [FileLink](T_TFlex_Model_FileLink.md)
    Файл с типом структуры изделия

#### Возвращаемое значение

[ProductStructure](T_TFlex_Model_ProductStructure.md)

#### Ссылки

[ProductStructure - ](T_TFlex_Model_ProductStructure.md)

[CreateProductStructure - перегрузка](Overload_TFlex_Model_ProductStructure_CreateProductStructure.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
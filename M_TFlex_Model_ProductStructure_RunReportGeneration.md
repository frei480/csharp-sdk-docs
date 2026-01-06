

Руководство по T-FLEX CAD Open API

# ProductStructureRunReportGeneration - метод  
    
Запустить генерацию отчета структуры изделия

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void RunReportGeneration(
	Guid reportID,
	ProductStructureReportOptions options
)
```
```vb
Public Sub RunReportGeneration ( 
	reportID As Guid,
	options As ProductStructureReportOptions
)
```
```cpp
public:
void RunReportGeneration(
	Guid reportID, 
	ProductStructureReportOptions^ options
)
```


#### Параметры

reportID [Guid](https://learn.microsoft.com/dotnet/api/system.guid)
    Идентификатор отчета. Можно получить из схемы структуры изделия.
options [ProductStructureReportOptions](T_TFlex_Model_ProductStructureReportOptions.md)
    Параметры генерации

#### Ссылки

[ProductStructure - ](T_TFlex_Model_ProductStructure.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
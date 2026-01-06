

Руководство по T-FLEX CAD Open API

# BOMObjectCreateStandardColumn - метод  
    
Создать колонку стандартного типа

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void CreateStandardColumn(
	string name,
	BOMObjectStandardField type,
	BOMObjectColumnSettings settings
)
```
```vb
Public Sub CreateStandardColumn ( 
	name As String,
	type As BOMObjectStandardField,
	settings As BOMObjectColumnSettings
)
```
```cpp
public:
void CreateStandardColumn(
	String^ name, 
	BOMObjectStandardField type, 
	BOMObjectColumnSettings^ settings
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название
type [BOMObjectStandardField](T_TFlex_Model_Model2D_BOMObject_StandardField.md)
    Тип
settings [BOMObjectColumnSettings](T_TFlex_Model_Model2D_BOMObject_ColumnSettings.md)
    Параметры колонки

#### Ссылки

[BOMObject - ](T_TFlex_Model_Model2D_BOMObject.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
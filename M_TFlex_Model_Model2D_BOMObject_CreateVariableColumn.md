

Руководство по T-FLEX CAD Open API

# BOMObjectCreateVariableColumn - метод  
  
---  
  
Создать колонку переменного типа

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void CreateVariableColumn(
	string name,
	string variableName,
	BOMObjectColumnSettings settings
)
```
```vb
Public Sub CreateVariableColumn ( 
	name As String,
	variableName As String,
	settings As BOMObjectColumnSettings
)
```
```cpp
public:
void CreateVariableColumn(
	String^ name, 
	String^ variableName, 
	BOMObjectColumnSettings^ settings
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название
variableName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя переменной, значение которой будет заносится в создаваемую колонку
settings [BOMObjectColumnSettings](T_TFlex_Model_Model2D_BOMObject_ColumnSettings.md)
    Параметры колонки

#### Ссылки

[BOMObject - ](T_TFlex_Model_Model2D_BOMObject.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
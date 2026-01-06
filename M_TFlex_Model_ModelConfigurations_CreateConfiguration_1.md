

Руководство по T-FLEX CAD Open API

# ModelConfigurationsCreateConfiguration(String, String, Boolean) - метод  
    
Создание конфигурации с именем name с текущим набором значений переменных

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool CreateConfiguration(
	string name,
	string variationName,
	bool isVariation
)
```
```vb
Public Function CreateConfiguration ( 
	name As String,
	variationName As String,
	isVariation As Boolean
) As Boolean
```
```cpp
public:
bool CreateConfiguration(
	String^ name, 
	String^ variationName, 
	bool isVariation
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя конфигурации
variationName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя исполнения
isVariation [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Тип - исполнение или конфигурация

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[ModelConfigurations - ](T_TFlex_Model_ModelConfigurations.md)

[CreateConfiguration - перегрузка](Overload_TFlex_Model_ModelConfigurations_CreateConfiguration.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
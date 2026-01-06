

Руководство по T-FLEX CAD Open API

# ParametersGetValueT \- метод  
    
Получить значение параметра с заданным ключом

**Пространство имён:** [TFlex.QualityManagement](N_TFlex_QualityManagement.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public T GetValue<T>(
	string key,
	T defaultValue
)

```




#### Параметры

key [String](https://learn.microsoft.com/dotnet/api/system.string)
    
defaultValue T
    

#### Параметры типа

T
    

#### Возвращаемое значение

TВозвращает defaultValue, если параметр не был найден или null при несоответствии типа параметра и запрашиваемого типа

#### Ссылки

[Parameters - ](T_TFlex_QualityManagement_Parameters.md)

[TFlex.QualityManagement - пространство имён](N_TFlex_QualityManagement.md)
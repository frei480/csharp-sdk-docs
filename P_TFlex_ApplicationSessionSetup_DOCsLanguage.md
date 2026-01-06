

Руководство по T-FLEX CAD Open API

# ApplicationSessionSetupDOCsLanguage - свойство  
    
Язык продукта T-FLEX DOCs, с которым необходимо установить интеграцию

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ApplicationLanguage DOCsLanguage { get; set; }
```
```vb
Public Property DOCsLanguage As ApplicationLanguage
	Get
	Set
```
```cpp
public:
property ApplicationLanguage DOCsLanguage {
	ApplicationLanguage get ();
	void set (ApplicationLanguage value);
}
```


#### Значение свойства

[ApplicationLanguage](T_TFlex_Application_Language.md)

Используйте значение [TFlex::Application::Language::Default](TFlex::Application::Language::Default) для интеграции с T-FLEX DOCs той же языковой версии, что и T-FLEX CAD

#### Ссылки

[ApplicationSessionSetup - ](T_TFlex_ApplicationSessionSetup.md)

[TFlex - пространство имён](N_TFlex.md)
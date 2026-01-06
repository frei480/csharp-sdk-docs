

Руководство по T-FLEX CAD Open API

# ApplicationRunSystemCommand - метод  
    
Выполнить команду с ожиданием её завершения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static void RunSystemCommand(
	string commandName,
	[OptionalAttribute] ModelObject[] selectObjects,
	[OptionalAttribute] SystemCommandFinishedCallback commandFinished
)
```
```vb
Public Shared Sub RunSystemCommand ( 
	commandName As String,
	<OptionalAttribute> selectObjects As ModelObject(),
	<OptionalAttribute> commandFinished As SystemCommandFinishedCallback
)
```
```cpp
public:
static void RunSystemCommand(
	String^ commandName, 
	[OptionalAttribute] array<ModelObject^>^ selectObjects, 
	[OptionalAttribute] SystemCommandFinishedCallback^ commandFinished
)
```


#### Параметры

commandName [String](https://learn.microsoft.com/dotnet/api/system.string)
    
selectObjects [ModelObject](T_TFlex_Model_ModelObject.md) (Optional)
    
commandFinished [SystemCommandFinishedCallback](T_TFlex_SystemCommandFinishedCallback.md) (Optional)
    

Название команды в T-FLEX Open API отображается во всплывающей подсказке к кнопке команды в интерфейсе T-FLEX CAD. Для включения её отображения во всплывающей подсказке к кнопке команды необходимо в T-FLEX CAD включить опцию "Включить в подсказки имена команд в Open API".

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)


Руководство по T-FLEX CAD Open API

# SingleButton - конструктор  
  
---  
  
Конструктор

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public SingleButton(
	int CmdID,
	KeyCode keyCode,
	ButtonStyle style
)
```
```vb
Public Sub New ( 
	CmdID As Integer,
	keyCode As KeyCode,
	style As ButtonStyle
)
```
```cpp
public:
SingleButton(
	int CmdID, 
	KeyCode keyCode, 
	ButtonStyle style
)
```


#### Параметры

CmdID [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды, которая будет выполнятся при нажатии на кнопку
keyCode [KeyCode](T_TFlex_KeyCode.md)
    Код клавиатуры
style [ButtonStyle](T_TFlex_Command_Button_Style.md)
    Состояние одиночной кнопки

#### Ссылки

[SingleButton - ](T_TFlex_Command_SingleButton.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)
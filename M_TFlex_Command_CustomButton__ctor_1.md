

Руководство по T-FLEX CAD Open API

# CustomButton(Int32, KeyCode, String, ButtonStyle) - конструктор  
    
Конструктор

**Пространство имён:** [TFlex.Command](N_TFlex_Command.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public CustomButton(
	int nIcon,
	KeyCode keyCode,
	string title,
	ButtonStyle style
)
```
```vb
Public Sub New ( 
	nIcon As Integer,
	keyCode As KeyCode,
	title As String,
	style As ButtonStyle
)
```
```cpp
public:
CustomButton(
	int nIcon, 
	KeyCode keyCode, 
	String^ title, 
	ButtonStyle style
)
```


#### Параметры

nIcon [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор команды автоменю, под которым приложение зарегестрировало эту команду
keyCode [KeyCode](T_TFlex_KeyCode.md)
    Код клавиатуры
title [String](https://learn.microsoft.com/dotnet/api/system.string)
    Комментарии
style [ButtonStyle](T_TFlex_Command_Button_Style.md)
    Состояние кнопки

#### Ссылки

[CustomButton - ](T_TFlex_Command_CustomButton.md)

[CustomButton - перегрузка](Overload_TFlex_Command_CustomButton__ctor.md)

[TFlex.Command - пространство имён](N_TFlex_Command.md)


Руководство по T-FLEX CAD Open API

# RibbonButtonAddChildButton(Int32, String, Plugin, RibbonButtonStyle) - метод  
    
Добавляет кнопку в список кнопок, вложенных в эту

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public RibbonButton AddChildButton(
	int commandId,
	string caption,
	Plugin plugin,
	RibbonButtonStyle style
)
```
```vb
Public Function AddChildButton ( 
	commandId As Integer,
	caption As String,
	plugin As Plugin,
	style As RibbonButtonStyle
) As RibbonButton
```
```cpp
public:
RibbonButton^ AddChildButton(
	int commandId, 
	String^ caption, 
	Plugin^ plugin, 
	RibbonButtonStyle style
)
```


#### Параметры

commandId [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
caption [String](https://learn.microsoft.com/dotnet/api/system.string)
    
plugin [Plugin](T_TFlex_Plugin.md)
    
style [RibbonButtonStyle](T_TFlex_RibbonButtonStyle.md)
    

#### Возвращаемое значение

[RibbonButton](T_TFlex_RibbonButton.md)

#### Ссылки

[RibbonButton - ](T_TFlex_RibbonButton.md)

[AddChildButton - перегрузка](Overload_TFlex_RibbonButton_AddChildButton.md)

[TFlex - пространство имён](N_TFlex.md)
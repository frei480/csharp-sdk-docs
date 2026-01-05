

Руководство по T-FLEX CAD Open API

# RibbonGroupAddButton(Int32, String, Plugin, RibbonButtonStyle) - метод  
  
---  
  
Добавляет кнопку в эту группу

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public RibbonButton AddButton(
	int commandId,
	string caption,
	Plugin plugin,
	RibbonButtonStyle style
)
```
```vb
Public Function AddButton ( 
	commandId As Integer,
	caption As String,
	plugin As Plugin,
	style As RibbonButtonStyle
) As RibbonButton
```
```cpp
public:
RibbonButton^ AddButton(
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

[RibbonGroup - ](T_TFlex_RibbonGroup.md)

[AddButton - перегрузка](Overload_TFlex_RibbonGroup_AddButton.md)

[TFlex - пространство имён](N_TFlex.md)


Руководство по T-FLEX CAD Open API

# ModalDialogPageForms - свойство  
    
Доступ коллекции форм с контролами, которые отображаются на данной вкладке

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public IList<PropertiesWindowFormBase> Forms { get; }
```
```vb
Public ReadOnly Property Forms As IList(Of PropertiesWindowFormBase)
	Get
```
```cpp
public:
property IList<PropertiesWindowFormBase^>^ Forms {
	IList<PropertiesWindowFormBase^>^ get ();
}
```


#### Значение свойства

[IList](https://learn.microsoft.com/dotnet/api/system.collections.generic.ilist-1)[PropertiesWindowFormBase](T_TFlex_Command_PropertiesWindowFormBase.md)

Вкладка может содержать несколько форм, в этом случае они стыкуются по вертикали

#### Ссылки

[ModalDialogPage - ](T_TFlex_Dialogs_ModalDialogPage.md)

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)
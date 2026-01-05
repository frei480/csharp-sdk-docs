

Руководство по T-FLEX CAD Open API

# LayerLineWidth - свойство  
  
---  
  
Значение толщины линии

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter LineWidth { get; set; }
```
```vb
Public Property LineWidth As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ LineWidth {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)
    
    
    public static void SetLineWidth(ModelObject ob)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("Установка толщины линии");//Открытие блока изменений документа
    
       ob.LineWidth = 3;    
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[Layer - ](T_TFlex_Model_Layer.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)


Руководство по T-FLEX CAD Open API

# AreaLineWidth - свойство  
    
Толщина линии

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

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

Данный метод выполняет указанное действие только в случае, если способ заполнения контура имеет значение [AreaFillStyle](T_TFlex_Model_Model2D_AreaFillStyle.md).Hatch или [AreaFillStyle](T_TFlex_Model_Model2D_AreaFillStyle.md).Pattern.
    
    
    public static void SetLineWidth(ModelObject ob)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("Установка толщины линии");//Открытие блока изменений документа
    
       ob.LineWidth = 3;    
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[Area - ](T_TFlex_Model_Model2D_Area.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
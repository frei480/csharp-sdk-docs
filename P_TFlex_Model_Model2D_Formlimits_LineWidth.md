

Руководство по T-FLEX CAD Open API

# FormlimitsLineWidth - свойство  
    
Толщина линий объекта

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter LineWidth { get; set; }
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

[Formlimits - ](T_TFlex_Model_Model2D_Formlimits.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
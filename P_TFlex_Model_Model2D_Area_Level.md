

Руководство по T-FLEX CAD Open API

# AreaLevel - свойство  
    
Уровень объекта

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter Level { get; set; }
```




#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)
    
    
    public static void SetLevel(Object ob)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("Установка уровня");//Открытие блока изменений документа
    
       ob.Level = 3;//установка уровня    
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[Area - ](T_TFlex_Model_Model2D_Area.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
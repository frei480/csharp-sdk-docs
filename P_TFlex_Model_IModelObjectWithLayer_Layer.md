

Руководство по T-FLEX CAD Open API

# IModelObjectWithLayerLayer - свойство  
    
Слой, на котором размещается объект

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
Layer Layer { get; set; }
```




#### Значение свойства

[Layer](T_TFlex_Model_Layer.md)
    
    
    public static void SetLayer(Object ob)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       Layer l = new Layer(document);
       l.Monochrome = true;//Параметр слоя "одноцветный"
       l.Color = 12;//цвет
    
       ob.Layer = l;//установка слоя 
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[IModelObjectWithLayer - ](T_TFlex_Model_IModelObjectWithLayer.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
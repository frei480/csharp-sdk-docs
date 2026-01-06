

Руководство по T-FLEX CAD Open API

# BodyPartLayer - свойство  
    
Слой, на котором размещается объект

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Layer Layer { get; set; }
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

[BodyPart - ](T_TFlex_Model_Model3D_BodyPart.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
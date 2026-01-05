

Руководство по T-FLEX CAD Open API

# FormlimitsLeaderLayer - свойство  
  
---  
  
Слой, на котором размещается объект

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual Layer Layer { get; set; }
```
```vb
Public Overridable Property Layer As Layer
	Get
	Set
```
```cpp
public:
virtual property Layer^ Layer {
	Layer^ get ();
	void set (Layer^ value);
}
```


#### Значение свойства

[Layer](T_TFlex_Model_Layer.md)

#### Реализации

[IModelObjectWithLayerLayer](P_TFlex_Model_IModelObjectWithLayer_Layer.md)
    
    
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

[FormlimitsLeader - ](T_TFlex_Model_Model2D_FormlimitsLeader.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# ImportFromParasolidLayer - свойство  
  
---  
  
Задание слоя

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Layer Layer { get; set; }
```
```vb
Public Property Layer As Layer
	Get
	Set
```
```cpp
public:
property Layer^ Layer {
	Layer^ get ();
	void set (Layer^ value);
}
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

[ImportFromParasolid - ](T_TFlex_Model_ImportFromParasolid.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
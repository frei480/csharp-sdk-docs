

Руководство по T-FLEX CAD Open API

# NodeColor - свойство  
  
---  
  
Цвет объекта

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter Color { get; set; }
```
```vb
Public Property Color As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Color {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)
    
    
    public static void SetColor(Object ob)
    {            
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       ob.Color = 40;//установка цвета
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[Node - ](T_TFlex_Model_Model2D_Node.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
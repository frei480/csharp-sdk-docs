

Руководство по T-FLEX CAD Open API

# OutlinesIntersectionLevel - свойство  
  
---  
  
Уровень

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Parameter Level { get; set; }
```
```vb
Public Property Level As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Level {
	Parameter^ get ();
	void set (Parameter^ value);
}
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

[OutlinesIntersection - ](T_TFlex_Model_Model2D_OutlinesIntersection.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# FixingVectorPage - свойство  
  
---  
  
Страница, на которой размещается элемент

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public override Page Page { get; set; }
```
```vb
Public Overrides Property Page As Page
	Get
	Set
```
```cpp
public:
virtual property Page^ Page {
	Page^ get () override;
	void set (Page^ value) override;
}
```


#### Значение свойства

[Page](T_TFlex_Model_Page.md)
    
    
    public static void SetPage(ModelObject ob)
    {            
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       Page p = new Page(document);//создание страницы
       p.Name = "страница1"
       ob.Page = p;//cтраница, на которой размещается элемент
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[FixingVector - ](T_TFlex_Model_Model2D_FixingVector.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# Section3DPage - свойство  
    
Страница

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Page Page { get; set; }
```
```vb
Public Property Page As Page
	Get
	Set
```
```cpp
public:
property Page^ Page {
	Page^ get ();
	void set (Page^ value);
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

[Section3D - ](T_TFlex_Model_Model3D_Section3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
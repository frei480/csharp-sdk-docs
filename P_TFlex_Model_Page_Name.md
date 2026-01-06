

Руководство по T-FLEX CAD Open API

# PageName - свойство  
    
Имя страницы

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public override string Name { get; set; }
```
```vb
Public Overrides Property Name As String
	Get
	Set
```
```cpp
public:
virtual property String^ Name {
	String^ get () override;
	void set (String^ value) override;
}
```


#### Значение свойства

[String](https://learn.microsoft.com/dotnet/api/system.string)
    
    
    public static void SetName(String name) 
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       //получение объекта по имени
       ModelObject ob = document.GetObjectByName("x");
       if(ob!= null)
       {
        //назначить имя объекту
        ob.Name = "a1";
       }
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[Page - ](T_TFlex_Model_Page.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)


Руководство по T-FLEX CAD Open API

# ModelObjectName - свойство  
  
---  
  
Имя объекта

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public virtual string Name { get; set; }
```
```vb
Public Overridable Property Name As String
	Get
	Set
```
```cpp
public:
virtual property String^ Name {
	String^ get ();
	void set (String^ value);
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

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
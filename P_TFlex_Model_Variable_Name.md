

Руководство по T-FLEX CAD Open API

# VariableName - свойство  
    
Имя переменной

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

Если после переименования требуется обновить имя данной переменной в выражениях других переменных, используйте вместо данного свойства метод RenameName
    
    
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

[Variable - ](T_TFlex_Model_Variable.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
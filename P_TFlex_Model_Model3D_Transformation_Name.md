

Руководство по T-FLEX CAD Open API

# TransformationName - свойство  
  
---  
  
Имя преобразования

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

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

Имя преобразования уникальное для элемента содержащего это преобразование
    
    
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

[Transformation - ](T_TFlex_Model_Model3D_Transformation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
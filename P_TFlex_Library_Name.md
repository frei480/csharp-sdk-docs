

Руководство по T-FLEX CAD Open API

# LibraryName - свойство  
    
Название библиотеки

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public string Name { get; set; }
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

[Library - ](T_TFlex_Library.md)

[TFlex - пространство имён](N_TFlex.md)
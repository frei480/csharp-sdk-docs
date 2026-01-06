

Руководство по T-FLEX CAD Open API

# ModelObjectID - свойство  
    
**Примечание: Данный API устарел.**

Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This property is obsolete and will be removed. Please use 'ObjectId' property.")]
public uint ID { get; }
```




#### Значение свойства

[UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    
    
    public static void ID(UInt32 ID)
    {            
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       if(document.GetObjectByID(ID)!= null)//получение объекта по идентификатору
       {
        //действия с объектом    
       }
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
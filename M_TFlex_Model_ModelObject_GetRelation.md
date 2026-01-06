

Руководство по T-FLEX CAD Open API

# ModelObjectGetRelation - метод  
    
Измерить отношение двух объектов

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public double? GetRelation(
	ModelObject other,
	string relationName
)
```




#### Параметры

other [ModelObject](T_TFlex_Model_ModelObject.md)
    Второй объект
relationName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя параметра для измерения, например Distance (см. команду Измерить в пользовательском интерфейсе)

#### Возвращаемое значение

[Nullable](https://learn.microsoft.com/dotnet/api/system.nullable-1)[Double](https://learn.microsoft.com/dotnet/api/system.double)

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
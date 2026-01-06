

Руководство по T-FLEX CAD Open API

# DocumentGetClosestObject(Point, Page, SelectionFilter) - метод  
    
Получить объект, ближайший к заданной точке на заданной странице с учётом фильтра

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ModelObject GetClosestObject(
	Point point,
	Page page,
	SelectionFilter filter
)
```




#### Параметры

point [Point](T_TFlex_Drawing_Point.md)
    Точка на чертеже
page [Page](T_TFlex_Model_Page.md)
    Страница чертежа
filter [SelectionFilter](T_TFlex_Model_SelectionFilter.md)
    Фильтр объектов

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)Найденный объект или null если объект не найден

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[GetClosestObject - перегрузка](Overload_TFlex_Model_Document_GetClosestObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
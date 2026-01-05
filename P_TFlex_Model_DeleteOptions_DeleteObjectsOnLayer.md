

Руководство по T-FLEX CAD Open API

# DeleteOptionsDeleteObjectsOnLayer - свойство  
  
---  
  
Используется методом DeleteObjects

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool DeleteObjectsOnLayer { get; set; }
```
```vb
Public Property DeleteObjectsOnLayer As Boolean
	Get
	Set
```
```cpp
public:
property bool DeleteObjectsOnLayer {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Задаёт удаление слоя и всех элементов, находящихся на нем. Если false, слой будет удален, если только на нем нет элементов.

#### Ссылки

[DeleteOptions - ](T_TFlex_Model_DeleteOptions.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
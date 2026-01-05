

Руководство по T-FLEX CAD Open API

# DeleteOptionsDeletePageObjects - свойство  
  
---  
  
Используется методом DeletePage

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool DeletePageObjects { get; set; }
```
```vb
Public Property DeletePageObjects As Boolean
	Get
	Set
```
```cpp
public:
property bool DeletePageObjects {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Задаёт удаление страницы и всех элементов, находящихся на ней. Если false, станица будет удалена, если только на ней нет элементов.

#### Ссылки

[DeleteOptions - ](T_TFlex_Model_DeleteOptions.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
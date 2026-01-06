

Руководство по T-FLEX CAD Open API

# PopupToolBarButtonSetAdd(Int32, Boolean) - метод  
    
Добавляет в этот набор кнопку с указанными параметрами

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool Add(
	int id,
	bool required
)
```
```vb
Public Function Add ( 
	id As Integer,
	required As Boolean
) As Boolean
```
```cpp
public:
bool Add(
	int id, 
	bool required
)
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор кнопки
required [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    true, если кнопка всегда должна отображаться в панели; false, если допускается расположение кнопки в расширенном меню

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)true, если кнопка была добавлена в этот набор; false, если указанный идентификатор некорректен или используется одной из кнопок, уже имеющихся в этом наборе

#### Ссылки

[PopupToolBarButtonSet - ](T_TFlex_PopupToolBarButtonSet.md)

[Add - перегрузка](Overload_TFlex_PopupToolBarButtonSet_Add.md)

[TFlex - пространство имён](N_TFlex.md)
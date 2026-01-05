

Руководство по T-FLEX CAD Open API

# ProxyObjectGetContextMenu - метод  
  
---  
  
Метод вызывается при вызове контекстного меню прокси объекта

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual bool GetContextMenu(
	Menu Menu
)
```
```vb
Protected Overridable Function GetContextMenu ( 
	Menu As Menu
) As Boolean
```
```cpp
protected:
virtual bool GetContextMenu(
	Menu^ Menu
)
```


#### Параметры

Menu [Menu](T_TFlex_Menu.md)
    Контекстное меню

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

В реализации данного метода можно добавить или удалить команды

#### Ссылки

[ProxyObject - ](T_TFlex_Model_ProxyObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
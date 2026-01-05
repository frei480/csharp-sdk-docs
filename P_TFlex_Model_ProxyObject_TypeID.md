

Руководство по T-FLEX CAD Open API

# ProxyObjectTypeID - свойство  
  
---  
  
Идентификатор типа объекта

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual int TypeID { get; }
```
```vb
Protected Overridable ReadOnly Property TypeID As Integer
	Get
```
```cpp
protected:
virtual property int TypeID {
	int get ();
}
```


#### Значение свойства

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

Тип объекта является уникальным в пределах приложения и не должен меняться. В соответствии с типом, система вызывает метод [CreateObject(Document, IntPtr, Int32)](M_TFlex_Plugin_CreateObject.md) для создания прокси объекта при чтении файла, выполнении отмены действий и т.д.

#### Ссылки

[ProxyObject - ](T_TFlex_Model_ProxyObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
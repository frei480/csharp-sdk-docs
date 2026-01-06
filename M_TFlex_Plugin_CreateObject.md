

Руководство по T-FLEX CAD Open API

# PluginCreateObject - метод  
    
Приложение переопределяет эту функцию для создания объекта модели указанного типа

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual ProxyObject CreateObject(
	Document __unnamed000,
	IntPtr OwnerHandle,
	int TypeID
)
```
```vb
Protected Overridable Function CreateObject ( 
	__unnamed000 As Document,
	OwnerHandle As IntPtr,
	TypeID As Integer
) As ProxyObject
```
```cpp
protected:
virtual ProxyObject^ CreateObject(
	Document^ __unnamed000, 
	IntPtr OwnerHandle, 
	int TypeID
)
```


#### Параметры

__unnamed000 [Document](T_TFlex_Model_Document.md)
    
OwnerHandle [IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)
    
TypeID [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Возвращаемое значение

[ProxyObject](T_TFlex_Model_ProxyObject.md)

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)
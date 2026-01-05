

Руководство по T-FLEX CAD Open API

# ProxyObjectRead - метод  
  
---  
  
Метод для считывания данных прокси объекта из файла

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
protected virtual void Read(
	Stream stream,
	int Version
)
```
```vb
Protected Overridable Sub Read ( 
	stream As Stream,
	Version As Integer
)
```
```cpp
protected:
virtual void Read(
	Stream^ stream, 
	int Version
)
```


#### Параметры

stream [Stream](https://learn.microsoft.com/dotnet/api/system.io.stream)
    Поток из которого происходит считывание данных
Version [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Версия объекта, на момент сохранения объекта в файл

#### Ссылки

[ProxyObject - ](T_TFlex_Model_ProxyObject.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
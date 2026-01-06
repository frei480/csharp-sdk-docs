

Руководство по T-FLEX CAD Open API

# ObjectTypeExtensionGetAsString - метод  
    
Получить локализованное имя типа объекта или null если имя не задано

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static string GetAsString(
	this ObjectType objectType
)
```
```vb
<ExtensionAttribute>
Public Shared Function GetAsString ( 
	objectType As ObjectType
) As String
```
```cpp
public:
[ExtensionAttribute]
static String^ GetAsString(
	ObjectType objectType
)
```


#### Параметры

objectType [ObjectType](T_TFlex_Model_ObjectType.md)
    

#### Возвращаемое значение

[String](https://learn.microsoft.com/dotnet/api/system.string)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [ObjectType](T_TFlex_Model_ObjectType.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[ObjectTypeExtension - ](T_TFlex_Model_ObjectTypeExtension.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
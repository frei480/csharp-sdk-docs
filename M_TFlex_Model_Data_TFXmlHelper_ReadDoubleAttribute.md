

Руководство по T-FLEX CAD Open API

# TFXmlHelperReadDoubleAttribute - метод  
  **Пространство имён:** [TFlex.Model.Data](N_TFlex_Model_Data.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public static double ReadDoubleAttribute(
	this XmlElement element,
	string attrName,
	double defValue = 0
)
```
```vb
<ExtensionAttribute>
Public Shared Function ReadDoubleAttribute ( 
	element As XmlElement,
	attrName As String,
	Optional defValue As Double = 0
) As Double
```
```cpp
public:
[ExtensionAttribute]
static double ReadDoubleAttribute(
	XmlElement^ element, 
	String^ attrName, 
	double defValue = 0
)
```


#### Параметры

element [XmlElement](https://learn.microsoft.com/dotnet/api/system.xml.xmlelement)
    
attrName [String](https://learn.microsoft.com/dotnet/api/system.string)
    
defValue [Double](https://learn.microsoft.com/dotnet/api/system.double) (Optional)
    

#### Возвращаемое значение

[Double](https://learn.microsoft.com/dotnet/api/system.double)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [XmlElement](https://learn.microsoft.com/dotnet/api/system.xml.xmlelement). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[TFXmlHelper - ](T_TFlex_Model_Data_TFXmlHelper.md)

[TFlex.Model.Data - пространство имён](N_TFlex_Model_Data.md)
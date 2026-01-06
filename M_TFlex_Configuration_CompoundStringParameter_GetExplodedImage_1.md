

Руководство по T-FLEX CAD Open API

# CompoundStringParameterGetExplodedImage(Document, String, Boolean, NullableColor) - метод  
  **Пространство имён:** [TFlex.Configuration](N_TFlex_Configuration.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Image GetExplodedImage(
	Document document,
	string str,
	bool explodeString,
	Color? backgroundColor
)
```
```vb
Public Shared Function GetExplodedImage ( 
	document As Document,
	str As String,
	explodeString As Boolean,
	backgroundColor As Color?
) As Image
```
```cpp
public:
static Image^ GetExplodedImage(
	Document^ document, 
	String^ str, 
	bool explodeString, 
	Nullable<Color> backgroundColor
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    
str [String](https://learn.microsoft.com/dotnet/api/system.string)
    
explodeString [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
backgroundColor [Nullable](https://learn.microsoft.com/dotnet/api/system.nullable-1)[Color](https://learn.microsoft.com/dotnet/api/system.drawing.color)
    

#### Возвращаемое значение

[Image](https://learn.microsoft.com/dotnet/api/system.drawing.image)

#### Ссылки

[CompoundStringParameter - ](T_TFlex_Configuration_CompoundStringParameter.md)

[GetExplodedImage - перегрузка](Overload_TFlex_Configuration_CompoundStringParameter_GetExplodedImage.md)

[TFlex.Configuration - пространство имён](N_TFlex_Configuration.md)
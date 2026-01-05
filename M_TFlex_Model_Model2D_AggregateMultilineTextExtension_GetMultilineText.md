

Руководство по T-FLEX CAD Open API

# AggregateMultilineTextExtensionGetMultilineText - метод  
  
---  
  
Получить аггрегированный многострочный текст

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static MultilineText GetMultilineText(
	this ModelObject __unnamed000,
	int idx,
	bool bForSet
)
```
```vb
<ExtensionAttribute>
Public Shared Function GetMultilineText ( 
	__unnamed000 As ModelObject,
	idx As Integer,
	bForSet As Boolean
) As MultilineText
```
```cpp
public:
[ExtensionAttribute]
static MultilineText^ GetMultilineText(
	ModelObject^ __unnamed000, 
	int idx, 
	bool bForSet
)
```


#### Параметры

__unnamed000 [ModelObject](T_TFlex_Model_ModelObject.md)
    
idx [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    
bForSet [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[MultilineText](T_TFlex_Model_Model2D_MultilineText.md)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [ModelObject](T_TFlex_Model_ModelObject.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[AggregateMultilineTextExtension - ](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
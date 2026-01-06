

Руководство по T-FLEX CAD Open API

# Document3DGetExternalOperations(Document, Int32) - метод  
    
Получить контейнер внешних операций документа

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static ExternalOperationCollection GetExternalOperations(
	this Document document,
	int typeId
)
```
```vb
<ExtensionAttribute>
Public Shared Function GetExternalOperations ( 
	document As Document,
	typeId As Integer
) As ExternalOperationCollection
```
```cpp
public:
[ExtensionAttribute]
static ExternalOperationCollection^ GetExternalOperations(
	Document^ document, 
	int typeId
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ
typeId [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Пользовательский идентификатор типа объекта

#### Возвращаемое значение

[ExternalOperationCollection](T_TFlex_Model_Model3D_ExternalOperationCollection.md)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [Document](T_TFlex_Model_Document.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[Document3D - ](T_TFlex_Model_Model3D_Document3D.md)

[GetExternalOperations - перегрузка](Overload_TFlex_Model_Model3D_Document3D_GetExternalOperations.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
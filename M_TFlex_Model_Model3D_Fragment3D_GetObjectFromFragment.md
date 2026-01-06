

Руководство по T-FLEX CAD Open API

# Fragment3DGetObjectFromFragment - метод  
  **Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Object3D GetObjectFromFragment(
	this Fragment3D fragment3D,
	string name,
	ICollection<ObjectId> subFragmentPath
)
```
```vb
<ExtensionAttribute>
Public Shared Function GetObjectFromFragment ( 
	fragment3D As Fragment3D,
	name As String,
	subFragmentPath As ICollection(Of ObjectId)
) As Object3D
```
```cpp
public:
[ExtensionAttribute]
static Object3D^ GetObjectFromFragment(
	Fragment3D^ fragment3D, 
	String^ name, 
	ICollection<ObjectId^>^ subFragmentPath
)
```


#### Параметры

fragment3D [Fragment3D](T_TFlex_Model_Model3D_Fragment3D.md)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    
subFragmentPath [ICollection](https://learn.microsoft.com/dotnet/api/system.collections.generic.icollection-1)[ObjectId](T_TFlex_Model_ObjectId.md)
    

#### Возвращаемое значение

[Object3D](T_TFlex_Model_Model3D_Object3D.md)

#### Примечание об использовании

В Visual Basic и C# этот метод можно вызывать как метод экземпляра для любого объекта типа [Fragment3D](T_TFlex_Model_Model3D_Fragment3D.md). При вызове метода для экземпляра следует опускать первый параметр. Дополнительные сведения см. в разделе [Методы расширения (Visual Basic)](https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods) или [Методы расширения (Руководство по программированию в C#)](https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods).

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
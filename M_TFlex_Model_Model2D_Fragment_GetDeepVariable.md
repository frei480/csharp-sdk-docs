

Руководство по T-FLEX CAD Open API

# FragmentGetDeepVariable - метод  
  **Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public DeepFragmentVariableValue GetDeepVariable(
	IEnumerable<ObjectId> fragmnetChainIds,
	string name
)
```
```vb
Public Function GetDeepVariable ( 
	fragmnetChainIds As IEnumerable(Of ObjectId),
	name As String
) As DeepFragmentVariableValue
```
```cpp
public:
DeepFragmentVariableValue^ GetDeepVariable(
	IEnumerable<ObjectId^>^ fragmnetChainIds, 
	String^ name
)
```


#### Параметры

fragmnetChainIds [IEnumerable](https://learn.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1)[ObjectId](T_TFlex_Model_ObjectId.md)
    
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    

#### Возвращаемое значение

[DeepFragmentVariableValue](T_TFlex_Model_DeepFragmentVariableValue.md)

#### Ссылки

[Fragment - ](T_TFlex_Model_Model2D_Fragment.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
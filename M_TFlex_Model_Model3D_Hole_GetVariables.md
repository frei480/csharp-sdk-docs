

Руководство по T-FLEX CAD Open API

# HoleGetVariables - метод  
  
---  
  
Получить переменные по индексу отверстия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ICollection<FragmentVariableValue> GetVariables(
	int hole
)
```
```vb
Public Function GetVariables ( 
	hole As Integer
) As ICollection(Of FragmentVariableValue)
```
```cpp
public:
ICollection<FragmentVariableValue^>^ GetVariables(
	int hole
)
```


#### Параметры

hole [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс отверстия

#### Возвращаемое значение

[ICollection](https://learn.microsoft.com/dotnet/api/system.collections.generic.icollection-1)[FragmentVariableValue](T_TFlex_Model_FragmentVariableValue.md)Переменные отверстия

#### Ссылки

[Hole - ](T_TFlex_Model_Model3D_Hole.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
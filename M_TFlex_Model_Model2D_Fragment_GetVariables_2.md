

Руководство по T-FLEX CAD Open API

# FragmentGetVariables(Boolean, Boolean) - метод  
  
---  
  
Контейнер переменных фрагмента

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ICollection<FragmentVariableValue> GetVariables(
	bool includeInternal,
	bool includeFixing
)
```
```vb
Public Function GetVariables ( 
	includeInternal As Boolean,
	includeFixing As Boolean
) As ICollection(Of FragmentVariableValue)
```
```cpp
public:
ICollection<FragmentVariableValue^>^ GetVariables(
	bool includeInternal, 
	bool includeFixing
)
```


#### Параметры

includeInternal [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Включить скрытые переменные
includeFixing [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Включить переменные фиксации (x1, y1 - x9, y9)

#### Возвращаемое значение

[ICollection](https://learn.microsoft.com/dotnet/api/system.collections.generic.icollection-1)[FragmentVariableValue](T_TFlex_Model_FragmentVariableValue.md)

#### Ссылки

[Fragment - ](T_TFlex_Model_Model2D_Fragment.md)

[GetVariables - перегрузка](Overload_TFlex_Model_Model2D_Fragment_GetVariables.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
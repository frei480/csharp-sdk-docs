

Руководство по T-FLEX CAD Open API

# FragmentGetBOMQuantity - метод  
    
Получить количество копий фрагмента в всех массивах

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int GetBOMQuantity(
	bool onlyVisible
)
```
```vb
Public Function GetBOMQuantity ( 
	onlyVisible As Boolean
) As Integer
```
```cpp
public:
int GetBOMQuantity(
	bool onlyVisible
)
```


#### Параметры

onlyVisible [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Считать количество только видимых копий, иначе считать все

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

#### Ссылки

[Fragment - ](T_TFlex_Model_Model2D_Fragment.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# Fragment3DGetBOMQuantity - метод  
  
---  
  
Получить количество копий фрагмента во всех массивах

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

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
    Считать количество только видимых копий, иначе считать всё

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Количество копий фрагмента во всех массивах

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
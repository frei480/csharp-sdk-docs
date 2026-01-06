

Руководство по T-FLEX CAD Open API

# FragmentGetFixingNode - метод  
    
Установка узла привязки точки привязки фрагмента, привязанного при помощи переменных привязки

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Node GetFixingNode(
	int index
)
```
```vb
Public Function GetFixingNode ( 
	index As Integer
) As Node
```
```cpp
public:
Node^ GetFixingNode(
	int index
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки привязки. Может иметь значение от 1 до 9

#### Возвращаемое значение

[Node](T_TFlex_Model_Model2D_Node.md)Узел, к которому привязаны точки привязки фрагмента

#### Ссылки

[Fragment - ](T_TFlex_Model_Model2D_Fragment.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# FragmentSetFixingNode - метод  
    
Установка узла привязки точки привязки фрагмента, привязанного при помощи переменных привязки

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetFixingNode(
	int index,
	Node node
)
```
```vb
Public Sub SetFixingNode ( 
	index As Integer,
	node As Node
)
```
```cpp
public:
void SetFixingNode(
	int index, 
	Node^ node
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки привязки. Может иметь значение от 1 до 9
node [Node](T_TFlex_Model_Model2D_Node.md)
    Узел, к которому привязана точка привязки фрагмента

Переменные привязки - переменные в документе фрагмента с имененем x или y и индексом от 1 до 9

#### Ссылки

[Fragment - ](T_TFlex_Model_Model2D_Fragment.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
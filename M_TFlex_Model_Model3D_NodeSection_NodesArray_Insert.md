

Руководство по T-FLEX CAD Open API

# NodeSectionNodesArrayInsert - метод  
    
Вставить узел перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int Index,
	Node node
)
```
```vb
Public Sub Insert ( 
	Index As Integer,
	node As Node
)
```
```cpp
public:
void Insert(
	int Index, 
	Node^ node
)
```


#### Параметры

Index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки
node [Node](T_TFlex_Model_Model2D_Node.md)
    

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат неопределён

#### Ссылки

[NodeSectionNodesArray - ](T_TFlex_Model_Model3D_NodeSection_NodesArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
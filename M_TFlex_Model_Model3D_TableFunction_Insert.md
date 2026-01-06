

Руководство по T-FLEX CAD Open API

# TableFunctionInsert - метод  
    
Вставить точку перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int index,
	TableFunctionDependence pair
)
```
```vb
Public Sub Insert ( 
	index As Integer,
	pair As TableFunctionDependence
)
```
```cpp
public:
void Insert(
	int index, 
	TableFunctionDependence^ pair
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки
pair [TableFunctionDependence](T_TFlex_Model_Model3D_TableFunction_Dependence.md)
    Пара независимого и зависимого параметра

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат не определён

#### Ссылки

[TableFunction - ](T_TFlex_Model_Model3D_TableFunction.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
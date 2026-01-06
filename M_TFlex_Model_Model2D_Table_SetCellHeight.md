

Руководство по T-FLEX CAD Open API

# TableSetCellHeight - метод  
    
Установка высоты ячейки

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCellHeight(
	uint cell,
	double height,
	SizeMode mode
)
```
```vb
Public Sub SetCellHeight ( 
	cell As UInteger,
	height As Double,
	mode As SizeMode
)
```
```cpp
public:
void SetCellHeight(
	unsigned int cell, 
	double height, 
	SizeMode mode
)
```


#### Параметры

cell [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Порядковый номер ячейки таблицы
height [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Новая высота ячейки
mode [SizeMode](T_TFlex_Model_Model2D_SizeMode.md)
    Режим высоты ячейки

Будет изменена высота всей строки, содержащей данную ячейку

#### Ссылки

[Table - ](T_TFlex_Model_Model2D_Table.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# RichTextSetCursor(PositionProperties, PositionTablePosition) - метод  
    
Установка положения курсора в ячейке таблицы

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetCursor(
	PositionProperties position,
	PositionTablePosition table
)
```
```vb
Public Sub SetCursor ( 
	position As PositionProperties,
	table As PositionTablePosition
)
```
```cpp
public:
void SetCursor(
	PositionProperties position, 
	PositionTablePosition table
)
```


#### Параметры

position [PositionProperties](T_TFlex_Model_Model2D_PositionProperties.md)
    Положение курсора в ячейке таблицы
table [PositionTablePosition](T_TFlex_Model_Model2D_Position_TablePosition.md)
    Положение ячейки

Функция устанавливает курсор в начало(конец) ячейки таблицы

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[SetCursor - перегрузка](Overload_TFlex_Model_Model2D_RichText_SetCursor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
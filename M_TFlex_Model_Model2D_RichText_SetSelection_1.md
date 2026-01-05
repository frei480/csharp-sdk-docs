

Руководство по T-FLEX CAD Open API

# RichTextSetSelection(Position, Position) - метод  
  
---  
  
Установка выделения фрагмента текста

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetSelection(
	Position pos1,
	Position pos2
)
```
```vb
Public Sub SetSelection ( 
	pos1 As Position,
	pos2 As Position
)
```
```cpp
public:
void SetSelection(
	Position pos1, 
	Position pos2
)
```


#### Параметры

pos1 [Position](T_TFlex_Model_Model2D_Position.md)
    Начало выделяемого фрагмента
pos2 [Position](T_TFlex_Model_Model2D_Position.md)
    Конец выделяемого фрагмента

Курсор устанавливается в конец выделяемого фрагмента

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[SetSelection - перегрузка](Overload_TFlex_Model_Model2D_RichText_SetSelection.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
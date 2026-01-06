

Руководство по T-FLEX CAD Open API

# LeaderNoteSetArrowOutlineLine - метод  
    
Установка параметров привязки стрелки к отрезку

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetArrowOutlineLine(
	Outline line,
	bool isOnEnd,
	Parameter offset
)
```
```vb
Public Sub SetArrowOutlineLine ( 
	line As Outline,
	isOnEnd As Boolean,
	offset As Parameter
)
```
```cpp
public:
void SetArrowOutlineLine(
	Outline^ line, 
	bool isOnEnd, 
	Parameter^ offset
)
```


#### Параметры

line [Outline](T_TFlex_Model_Model2D_Outline.md)
    Отрезок привязки
isOnEnd [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Указывает на то, что привязка происходит к концу отрезка (иначе - к началу)
offset [Parameter](T_TFlex_Model_Parameter.md)
    Смещение точки привязки по отрезку относительно выбранного конца отрезка

#### Ссылки

[LeaderNote - ](T_TFlex_Model_Model2D_LeaderNote.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
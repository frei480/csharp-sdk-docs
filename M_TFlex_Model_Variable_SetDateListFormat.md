

Руководство по T-FLEX CAD Open API

# VariableSetDateListFormat - метод  
    
Установить формат даты

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetDateListFormat(
	string format
)
```
```vb
Public Sub SetDateListFormat ( 
	format As String
)
```
```cpp
public:
void SetDateListFormat(
	String^ format
)
```


#### Параметры

format [String](https://learn.microsoft.com/dotnet/api/system.string)
    Формат даты

Формат даты: "d" День месяца в виде одной или двух цифр, "dd" День месяца в виде двух цифр, "ddd" День недели в виде трёх букв, "dddd" Полное название дня недели, "M" Номер месяца в виде одной или двух цифр, "MM" Номер месяца в виде двух цифр, "MMM" Месяц в виде трёх букв, "MMMM" Полное название месяца, "y" Последняя цифра года, "yy" Последние две цифры года, "yyy" Полный год. 

#### Ссылки

[Variable - ](T_TFlex_Model_Variable.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
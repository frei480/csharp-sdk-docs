

Руководство по T-FLEX CAD Open API

# RichTextGetText - метод  
  
---  
  
Получение текста, находящегося в заданном отрезке

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public string GetText(
	Position pos1,
	Position pos2
)
```
```vb
Public Function GetText ( 
	pos1 As Position,
	pos2 As Position
) As String
```
```cpp
public:
String^ GetText(
	Position pos1, 
	Position pos2
)
```


#### Параметры

pos1 [Position](T_TFlex_Model_Model2D_Position.md)
    Начало отрезка
pos2 [Position](T_TFlex_Model_Model2D_Position.md)
    Конец отрезка

#### Возвращаемое значение

[String](https://learn.microsoft.com/dotnet/api/system.string)Текст, находящийся в заданном отрезке

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
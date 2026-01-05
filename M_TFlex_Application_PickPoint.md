

Руководство по T-FLEX CAD Open API

# ApplicationPickPoint(Document, PickPointParameters) - метод  
  
---  
  
Получить точку в одном из видов документа

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static PickPointResult PickPoint(
	Document document,
	PickPointParameters parameters
)
```
```vb
Public Shared Function PickPoint ( 
	document As Document,
	parameters As PickPointParameters
) As PickPointResult
```
```cpp
public:
static PickPointResult^ PickPoint(
	Document^ document, 
	PickPointParameters^ parameters
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ
parameters [PickPointParameters](T_TFlex_PickPointParameters.md)
    Параметры ввода точки

#### Возвращаемое значение

[PickPointResult](T_TFlex_PickPointResult.md)Результат ввода точки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[PickPoint - перегрузка](Overload_TFlex_Application_PickPoint.md)

[TFlex - пространство имён](N_TFlex.md)
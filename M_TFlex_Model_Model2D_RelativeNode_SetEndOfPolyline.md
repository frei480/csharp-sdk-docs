

Руководство по T-FLEX CAD Open API

# RelativeNodeSetEndOfPolyline - метод  
  
---  
  
Установка привязки к одному из концов линии построения - полилинии

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetEndOfPolyline(
	Construction srcConstruction,
	bool alignToStart
)
```
```vb
Public Sub SetEndOfPolyline ( 
	srcConstruction As Construction,
	alignToStart As Boolean
)
```
```cpp
public:
void SetEndOfPolyline(
	Construction^ srcConstruction, 
	bool alignToStart
)
```


#### Параметры

srcConstruction [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная линия построения
alignToStart [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр для определения положения узла

#### Ссылки

[RelativeNode - ](T_TFlex_Model_Model2D_RelativeNode.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# RelativeNodeSetByParameter - метод  
  
---  
  
Установка привязки к линии построения (Окружность, Эллипс, Полилиния) по параметру

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetByParameter(
	Construction srcConstruction,
	Parameter param
)
```
```vb
Public Sub SetByParameter ( 
	srcConstruction As Construction,
	param As Parameter
)
```
```cpp
public:
void SetByParameter(
	Construction^ srcConstruction, 
	Parameter^ param
)
```


#### Параметры

srcConstruction [Construction](T_TFlex_Model_Model2D_Construction.md)
    Исходная линия построения
param [Parameter](T_TFlex_Model_Parameter.md)
    Параметр для определения положения узла

#### Ссылки

[RelativeNode - ](T_TFlex_Model_Model2D_RelativeNode.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
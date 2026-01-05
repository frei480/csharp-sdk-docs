

Руководство по T-FLEX CAD Open API

# ConstructionDimensionSetOffsets - метод  
  
---  
  
Установка привязок размера к узлам, либо по относительным смещениям

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetOffsets(
	Node fixNodeX,
	double offsetX,
	Node fixNodeY,
	double offsetY
)
```
```vb
Public Sub SetOffsets ( 
	fixNodeX As Node,
	offsetX As Double,
	fixNodeY As Node,
	offsetY As Double
)
```
```cpp
public:
void SetOffsets(
	Node^ fixNodeX, 
	double offsetX, 
	Node^ fixNodeY, 
	double offsetY
)
```


#### Параметры

fixNodeX [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел привязки, смещение размера от точки привязки по горизонтали
offsetX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размера от точки привязки по горизонтали (используется, если fixNodeX не задан)
fixNodeY [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел привязки, смещение размера от точки привязки по вертикали
offsetY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размера от точки привязки по вертикали (используется, если fixNodeY не задан)

#### Ссылки

[ConstructionDimension - ](T_TFlex_Model_Model2D_ConstructionDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
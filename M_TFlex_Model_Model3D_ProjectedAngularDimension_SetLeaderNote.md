

Руководство по T-FLEX CAD Open API

# ProjectedAngularDimensionSetLeaderNote - метод  
  
---  
  
Установка привязок размера к узлам, либо по относительным смещениям

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetLeaderNote(
	Node fixNode1,
	double offset1,
	Node fixLeaderNode,
	double dX,
	double dY
)
```
```vb
Public Sub SetLeaderNote ( 
	fixNode1 As Node,
	offset1 As Double,
	fixLeaderNode As Node,
	dX As Double,
	dY As Double
)
```
```cpp
public:
void SetLeaderNote(
	Node^ fixNode1, 
	double offset1, 
	Node^ fixLeaderNode, 
	double dX, 
	double dY
)
```


#### Параметры

fixNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел привязки, задаёт положение размерной линии
offset1 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерной линии относительно начала первой выносной линии (используется, если fixNode1 не задан)
fixLeaderNode [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел привязки, задаёт положение выносной полки
dX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение по горизонтали конца выносной полки относительно середины размерной линии (используется, если fixLeaderNode не задан)
dY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение по вертикали конца выносной полки относительно середины размерной линии (используется, если fixLeaderNode не задан)

#### Ссылки

[ProjectedAngularDimension - ](T_TFlex_Model_Model3D_ProjectedAngularDimension.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
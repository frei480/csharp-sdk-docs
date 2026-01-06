

Руководство по T-FLEX CAD Open API

# ProjectedAngularDimensionSetOffsets - метод  
    
Установка привязок размера к узлам, либо по относительным смещениям

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetOffsets(
	Node fixNode1,
	double offset1,
	Node fixNode2,
	double offset2,
	Node fixNode3,
	double offset3
)
```
```vb
Public Sub SetOffsets ( 
	fixNode1 As Node,
	offset1 As Double,
	fixNode2 As Node,
	offset2 As Double,
	fixNode3 As Node,
	offset3 As Double
)
```
```cpp
public:
void SetOffsets(
	Node^ fixNode1, 
	double offset1, 
	Node^ fixNode2, 
	double offset2, 
	Node^ fixNode3, 
	double offset3
)
```


#### Параметры

fixNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел привязки, задаёт положение размерной линии
offset1 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерной линии относительно начала первой выносной линии (используется, если fixNode1 не задан)
fixNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел привязки, задаёт положение размерного числа
offset2 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерного числа относительно середины размерной линии (используется, если fixNode2 не задан)
fixNode3 [Node](T_TFlex_Model_Model2D_Node.md)
    Третий узел привязки, задаёт положения конца полки размера
offset3 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение длины полки размера (используется, если fixNode3 не задан)

#### Ссылки

[ProjectedAngularDimension - ](T_TFlex_Model_Model3D_ProjectedAngularDimension.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
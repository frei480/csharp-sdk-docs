

Руководство по T-FLEX CAD Open API

# LinearDimensionSetOffsets - метод  
    
Установка привязок размера к узлам, либо по относительным смещениям

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

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




#### Параметры

fixNode1 [Node](T_TFlex_Model_Model2D_Node.md)
    Первый узел привязки, задает положение размерной линии
offset1 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерной линии относительно начала первой выносной линии (используется, если fixNode1 не задан)
fixNode2 [Node](T_TFlex_Model_Model2D_Node.md)
    Второй узел привязки, задает положение размерного числа
offset2 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерного числа относительно середины размерной линии (используется, если fixNode2 не задан)
fixNode3 [Node](T_TFlex_Model_Model2D_Node.md)
    Третий узел привязки, задает положения конца полки размера
offset3 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение длины полки размера (используется, если fixNode3 не задан)

#### Ссылки

[LinearDimension - ](T_TFlex_Model_Model2D_LinearDimension.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
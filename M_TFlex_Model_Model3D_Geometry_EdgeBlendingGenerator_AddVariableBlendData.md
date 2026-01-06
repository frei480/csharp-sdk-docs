

Руководство по T-FLEX CAD Open API

# EdgeBlendingGeneratorAddVariableBlendData - метод  
    
Функция задаёт параметры для сглаживания ребра переменного радиуса

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddVariableBlendData(
	BaseTopol entity,
	double startsetback,
	double endsetback,
	int BlndStatus,
	int szvardata,
	double[] varBlndParam,
	double[] vradDataL,
	double[] vradDataR,
	double[] vradDataRHO
)
```
```vb
Public Sub AddVariableBlendData ( 
	entity As BaseTopol,
	startsetback As Double,
	endsetback As Double,
	BlndStatus As Integer,
	szvardata As Integer,
	varBlndParam As Double(),
	vradDataL As Double(),
	vradDataR As Double(),
	vradDataRHO As Double()
)
```
```cpp
public:
void AddVariableBlendData(
	BaseTopol^ entity, 
	double startsetback, 
	double endsetback, 
	int BlndStatus, 
	int szvardata, 
	array<double>^ varBlndParam, 
	array<double>^ vradDataL, 
	array<double>^ vradDataR, 
	array<double>^ vradDataRHO
)
```


#### Параметры

entity [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)
    Ребро для установки параметров сглаживания
startsetback [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение от вершины в начале ребра для создания "чемоданного угла"
endsetback [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение от вершины в конце ребра для создания "чемоданного угла"
BlndStatus [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Параметр режима сглаживания
szvardata [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Количество точек для задания радиус-функции
varBlndParam [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Массив значений параметров на ребре в процентах
vradDataL [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Массив значений радиусов/смещений по "левой" грани (по направлению ребра)
vradDataR [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Массив значений радиусов/смещений по "правой" грани (по направлению ребра)
vradDataRHO [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Массив значений параметров параметров формы сечения сглаживания на ребре (0. - круговое, ]0,0.5[ - эллиптическое, 0.5 - параболическое, ]0.5,1.[ - гиперболическое

#### Ссылки

[EdgeBlendingGenerator - ](T_TFlex_Model_Model3D_Geometry_EdgeBlendingGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
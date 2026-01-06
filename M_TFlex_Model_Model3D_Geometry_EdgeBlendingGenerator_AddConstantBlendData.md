

Руководство по T-FLEX CAD Open API

# EdgeBlendingGeneratorAddConstantBlendData - метод  
    
Функция задаёт параметры для сглаживания ребра постоянного радиуса

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddConstantBlendData(
	BaseTopol entity,
	double RF,
	double RS,
	double startsetback,
	double endsetback,
	int BlndStatus
)
```
```vb
Public Sub AddConstantBlendData ( 
	entity As BaseTopol,
	RF As Double,
	RS As Double,
	startsetback As Double,
	endsetback As Double,
	BlndStatus As Integer
)
```
```cpp
public:
void AddConstantBlendData(
	BaseTopol^ entity, 
	double RF, 
	double RS, 
	double startsetback, 
	double endsetback, 
	int BlndStatus
)
```


#### Параметры

entity [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)
    Топологический элемент для установки параметров сглаживания (ребро, грань, цикл или вершина)
RF [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Радиус сглаживания/смещение по первой грани для фаски
RS [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение по второй грани для фаски
startsetback [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение от вершины в начале ребра для создания "чемоданного угла"
endsetback [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение от вершины в конце ребра для создания "чемоданного угла"
BlndStatus [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Параметр режима сглаживания

#### Ссылки

[EdgeBlendingGenerator - ](T_TFlex_Model_Model3D_Geometry_EdgeBlendingGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
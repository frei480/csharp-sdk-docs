

Руководство по T-FLEX CAD Open API

# CircularDimension3DSetElement - метод  
    
Установка привязок размера к 3D элементам

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetElement(
	Object3D CircleElement,
	DimensionUVCoords Coords,
	bool Diameter,
	double Angle,
	double Offset
)
```
```vb
Public Sub SetElement ( 
	CircleElement As Object3D,
	Coords As DimensionUVCoords,
	Diameter As Boolean,
	Angle As Double,
	Offset As Double
)
```
```cpp
public:
void SetElement(
	Object3D^ CircleElement, 
	DimensionUVCoords^ Coords, 
	bool Diameter, 
	double Angle, 
	double Offset
)
```


#### Параметры

CircleElement [Object3D](T_TFlex_Model_Model3D_Object3D.md)
    Элемент для привязки размера (грань, ребро)
Coords [DimensionUVCoords](T_TFlex_Model_Model3D_DimensionUVCoords.md)
    Координаты для определения привязки размера
Diameter [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Ставим диаметр, если true, иначе - радиус
Angle [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Угол, на котором находится размерная стрелка
Offset [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Расстояние от размерного числа до окружности

#### Ссылки

[CircularDimension3D - ](T_TFlex_Model_Model3D_CircularDimension3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
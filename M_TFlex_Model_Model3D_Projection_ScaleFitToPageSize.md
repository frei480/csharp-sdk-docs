

Руководство по T-FLEX CAD Open API

# ProjectionScaleFitToPageSize - метод  
    
Подбор масшатаба для проекции, чтобы умещаться на странице

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public double ScaleFitToPageSize(
	double dPageWidth,
	double dPageHeight
)
```
```vb
Public Function ScaleFitToPageSize ( 
	dPageWidth As Double,
	dPageHeight As Double
) As Double
```
```cpp
public:
double ScaleFitToPageSize(
	double dPageWidth, 
	double dPageHeight
)
```


#### Параметры

dPageWidth [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
dPageHeight [Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Double](https://learn.microsoft.com/dotnet/api/system.double)Возвращает отрицательное значение, если не удалось подобрать масштаб

#### Ссылки

[Projection - ](T_TFlex_Model_Model3D_Projection.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
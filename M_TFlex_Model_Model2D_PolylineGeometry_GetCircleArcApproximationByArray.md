

Руководство по T-FLEX CAD Open API

# PolylineGeometryGetCircleArcApproximationByArray - метод  
    
Аппроксимация дугами окружности.

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static double[] GetCircleArcApproximationByArray(
	double[] X,
	double[] Y,
	double accuracy
)
```




#### Параметры

X [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
Y [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
accuracy [Double](https://learn.microsoft.com/dotnet/api/system.double)
    

#### Возвращаемое значение

[Double](https://learn.microsoft.com/dotnet/api/system.double)

Каждые шесть элементов (xb, yb, xm, ym, xe, ye) задают дугу.

#### Ссылки

[PolylineGeometry - ](T_TFlex_Model_Model2D_PolylineGeometry.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
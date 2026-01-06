

Руководство по T-FLEX CAD Open API

# AngularDimension3DSetOffsets - метод  
    
Установка привязок размера по относительным смещениям

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetOffsets(
	double Offset1,
	double Offset2,
	double Offset3
)
```
```vb
Public Sub SetOffsets ( 
	Offset1 As Double,
	Offset2 As Double,
	Offset3 As Double
)
```
```cpp
public:
void SetOffsets(
	double Offset1, 
	double Offset2, 
	double Offset3
)
```


#### Параметры

Offset1 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерной линии относительно начала первой выносной линии
Offset2 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерного числа относительно середины размерной линии
Offset3 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение - длина полки размера

#### Ссылки

[AngularDimension3D - ](T_TFlex_Model_Model3D_AngularDimension3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# AngularDimension3DSetLeaderNote - метод  
    
Установка привязок размера по относительным смещениям

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetLeaderNote(
	double Offset1,
	double dX,
	double dY
)
```
```vb
Public Sub SetLeaderNote ( 
	Offset1 As Double,
	dX As Double,
	dY As Double
)
```
```cpp
public:
void SetLeaderNote(
	double Offset1, 
	double dX, 
	double dY
)
```


#### Параметры

Offset1 [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение размерной линии относительно начала первой выносной линии
dX [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение по горизонтали конца выносной полки относительно середины размерной линии
dY [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Смещение по вертикали конца выносной полки относительно середины размерной линии

#### Ссылки

[AngularDimension3D - ](T_TFlex_Model_Model3D_AngularDimension3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
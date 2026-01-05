

Руководство по T-FLEX CAD Open API

# AffineMapToWCS - метод  
  
---  
  
Применить афинное преобразование

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void ToWCS(
	ref double x,
	ref double y
)
```
```vb
Public Sub ToWCS ( 
	ByRef x As Double,
	ByRef y As Double
)
```
```cpp
public:
void ToWCS(
	double% x, 
	double% y
)
```


#### Параметры

x [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата x точки в исходной системе координат
y [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата y точки в исходной системе координат

Входные значения координат x и y передаются по ссылке, на выходе метода получаем значения x и y в преобразованной системе координат

#### Ссылки

[AffineMap - ](T_TFlex_Drawing_AffineMap.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
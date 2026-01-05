

Руководство по T-FLEX CAD Open API

# GraphicsFontSpacing - свойство  
  
---  
  
Установка дополнительного интервала между символами

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public double FontSpacing { get; set; }
```
```vb
Public Property FontSpacing As Double
	Get
	Set
```
```cpp
public:
property double FontSpacing {
	double get ();
	void set (double value);
}
```


#### Значение свойства

[Double](https://learn.microsoft.com/dotnet/api/system.double)

Абсолютное значение дополнительного интервала между символами вычисляется перемножением высоты шрифта и данного коэффициента. По умолчанию коэффициент дополнительного интервала между символами шрифта равен 0

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
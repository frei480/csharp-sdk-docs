

Руководство по T-FLEX CAD Open API

# GraphicsFontInterval - свойство  
  
---  
  
Установка коэффициента междустрочного интервала

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public double FontInterval { get; set; }
```
```vb
Public Property FontInterval As Double
	Get
	Set
```
```cpp
public:
property double FontInterval {
	double get ();
	void set (double value);
}
```


#### Значение свойства

[Double](https://learn.microsoft.com/dotnet/api/system.double)

Абсолютное значение междустрочного интервала вычисляется перемножением высоты шрифта и данного коэффициента. По умолчанию коэффициент дополнительного интервала между симолами шрифта равен 0.5

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
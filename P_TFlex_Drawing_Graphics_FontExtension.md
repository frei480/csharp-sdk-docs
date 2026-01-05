

Руководство по T-FLEX CAD Open API

# GraphicsFontExtension - свойство  
  
---  
  
Установка коэффициента расширения шрифта

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public double FontExtension { get; set; }
```
```vb
Public Property FontExtension As Double
	Get
	Set
```
```cpp
public:
property double FontExtension {
	double get ();
	void set (double value);
}
```


#### Значение свойства

[Double](https://learn.microsoft.com/dotnet/api/system.double)

Коэффициент расширения шрифта учитывается только при выводе шрифта формата SHX. По умолчанию коэффициент расширения шрифта равен 1.

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
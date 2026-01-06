

Руководство по T-FLEX CAD Open API

# GraphicsArrowPolyline - метод  
    
Прорисовка полилинии со стрелками

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void ArrowPolyline(
	Polyline polyline,
	int startType,
	double startSize,
	int endType,
	double endSize
)
```




#### Параметры

polyline [Polyline](T_TFlex_Drawing_Polyline.md)
    Полилиния
startType [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Тип стрелки в начальной точке
startSize [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Размер стрелки в начальной точке
endType [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Тип стрелки в конечной точке
endSize [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Размер стрелки в конечной точке

Полилиния выводится с учётом установленной растровой операции, цвета вывода, толщины линий, типа линий

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
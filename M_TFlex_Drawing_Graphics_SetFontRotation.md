

Руководство по T-FLEX CAD Open API

# GraphicsSetFontRotation - метод  
    
Установка угла поворота текста с помощью вектора вертикали

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetFontRotation(
	double dx,
	double dy
)
```




#### Параметры

dx [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата x вектора вертикали шрифта
dy [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата y вектора вертикали шрифта

Для вывода обычного горизонтального текста вектор вертикали шрифта должен быть направлен вверх, например иметь координаты (1,0). Альтернативным способом задания угла поворота текста является свойство [FontAngle](P_TFlex_Drawing_Graphics_FontAngle.md)

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)


Руководство по T-FLEX CAD Open API

# GraphicsGetLinePatternPreview - метод  
  
---  
  
Получение изображения для предпросмотра стиля линии

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Bitmap GetLinePatternPreview(
	string pattern,
	ref Rectangle rect,
	Color backColor
)
```
```vb
Public Shared Function GetLinePatternPreview ( 
	pattern As String,
	ByRef rect As Rectangle,
	backColor As Color
) As Bitmap
```
```cpp
public:
static Bitmap^ GetLinePatternPreview(
	String^ pattern, 
	Rectangle% rect, 
	Color backColor
)
```


#### Параметры

pattern [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название стиля линии
rect [Rectangle](https://learn.microsoft.com/dotnet/api/system.drawing.rectangle)
    Область рисования
backColor [Color](https://learn.microsoft.com/dotnet/api/system.drawing.color)
    Цвет фона

#### Возвращаемое значение

[Bitmap](https://learn.microsoft.com/dotnet/api/system.drawing.bitmap)

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
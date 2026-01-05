

Руководство по T-FLEX CAD Open API

# GraphicsDrawBitmap - метод  
  
---  
**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void DrawBitmap(
	IntPtr bitmapHandle,
	double x,
	double y,
	double width,
	double height,
	double sin,
	double cos,
	Color? transparentColor,
	bool useAlphaChannel
)
```
```vb
Public Sub DrawBitmap ( 
	bitmapHandle As IntPtr,
	x As Double,
	y As Double,
	width As Double,
	height As Double,
	sin As Double,
	cos As Double,
	transparentColor As Color?,
	useAlphaChannel As Boolean
)
```
```cpp
public:
void DrawBitmap(
	IntPtr bitmapHandle, 
	double x, 
	double y, 
	double width, 
	double height, 
	double sin, 
	double cos, 
	Nullable<Color> transparentColor, 
	bool useAlphaChannel
)
```


#### Параметры

bitmapHandle [IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)
    
x [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
y [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
width [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
height [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
sin [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
cos [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
transparentColor [Nullable](https://learn.microsoft.com/dotnet/api/system.nullable-1)[Color](https://learn.microsoft.com/dotnet/api/system.drawing.color)
    
useAlphaChannel [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
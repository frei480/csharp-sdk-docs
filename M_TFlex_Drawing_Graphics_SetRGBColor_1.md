

Руководство по T-FLEX CAD Open API

# GraphicsSetRGBColor(Int32, Int32, Int32) - метод  
    
Установка цвета, которым должен производиться вывод, в виде компонент красного, зелёного и синего

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int SetRGBColor(
	int r,
	int g,
	int b
)
```
```vb
Public Function SetRGBColor ( 
	r As Integer,
	g As Integer,
	b As Integer
) As Integer
```
```cpp
public:
int SetRGBColor(
	int r, 
	int g, 
	int b
)
```


#### Параметры

r [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Красная составляющая (от 0 до 255)
g [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Зелёная составляющая (от 0 до 255)
b [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Синяя составляющая (от 0 до 255)

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Цвет, который был установлен до вызова данного метода

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[SetRGBColor - перегрузка](Overload_TFlex_Drawing_Graphics_SetRGBColor.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
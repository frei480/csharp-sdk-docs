

Руководство по T-FLEX CAD Open API

# StandardColorsFindClosestIndex(UInt32) - метод  
  
---  
  
Найти индекс, наиболее соответствующий данному цвету

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static int FindClosestIndex(
	uint colorref
)
```
```vb
Public Shared Function FindClosestIndex ( 
	colorref As UInteger
) As Integer
```
```cpp
public:
static int FindClosestIndex(
	unsigned int colorref
)
```


#### Параметры

colorref [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Цвет в формате Windows GDI (COLORREF)

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

Этот метод выполняется дольше, чем остальные методы класса, поэтому при возможности его результаты следует кэшировать.

#### Ссылки

[StandardColors - ](T_TFlex_Drawing_StandardColors.md)

[FindClosestIndex - перегрузка](Overload_TFlex_Drawing_StandardColors_FindClosestIndex.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
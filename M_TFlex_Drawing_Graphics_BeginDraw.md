

Руководство по T-FLEX CAD Open API

# GraphicsBeginDraw - метод  
  
---  
  
Начало вывода изображения

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void BeginDraw()
```
```vb
Public Sub BeginDraw
```
```cpp
public:
void BeginDraw()
```


Данный метод необходимо вызвать перед началом вывода изображения с использованием функций данного класса. Завершение вывода должно заканчиваться вызовом метода [EndDraw](M_TFlex_Drawing_Graphics_EndDraw.md). Вызовы этой пары функций могут быть вложенными, однако обязательным является соблюдение парности. Каждому вызову BeginDraw должен соответствовать вызов [EndDraw](M_TFlex_Drawing_Graphics_EndDraw.md).

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
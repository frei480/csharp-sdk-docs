

Руководство по T-FLEX CAD Open API

# Graphics - класс  
    
Класс предназначен для вывода графического изображения на экран или другое графическое устройство с использованием вещественных координат в системе координат документа.

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.DrawingGraphics

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class Graphics : IDisposable
```




Тип Graphics предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Graphics(Graphics, AffineMap)](M_TFlex_Drawing_Graphics__ctor_1.md) | Конструктор. Новый объект основанный на baseGraphics с применением к нему преобразования transformation. |
|  | [Graphics(IntPtr, Rectangle, Rectangle)](M_TFlex_Drawing_Graphics__ctor.md) | Конструктор |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [BkColor](P_TFlex_Drawing_Graphics_BkColor.md) | Цвет фона |
|  | [Color](P_TFlex_Drawing_Graphics_Color.md) | Цвет, которым производится вывод |
|  | [ColorLock](P_TFlex_Drawing_Graphics_ColorLock.md) | Режим запрета смены цвета (одноцветный режим) |
|  | [DashedPattern](P_TFlex_Drawing_Graphics_DashedPattern.md) |  |
|  | [DashedType](P_TFlex_Drawing_Graphics_DashedType.md) | Установка прорисовки шрихового типа линии |
|  | [DeviceContext](P_TFlex_Drawing_Graphics_DeviceContext.md) | Установка дескриптора графического устройства (HDC) |
|  | [FontAngle](P_TFlex_Drawing_Graphics_FontAngle.md) | Установка угла поворота текста |
|  | [FontClearBackground](P_TFlex_Drawing_Graphics_FontClearBackground.md) | Установка параметра "очистка фона" |
|  | [FontExtension](P_TFlex_Drawing_Graphics_FontExtension.md) | Установка коэффициента расширения шрифта |
|  | [FontHorizontalAlignment](P_TFlex_Drawing_Graphics_FontHorizontalAlignment.md) | Установка выравнивания текста по горизонтали |
|  | [FontInterval](P_TFlex_Drawing_Graphics_FontInterval.md) | Установка коэффициента междустрочного интервала |
|  | [FontName](P_TFlex_Drawing_Graphics_FontName.md) | Выбор шрифта для прорисовки текста |
|  | [FontSize](P_TFlex_Drawing_Graphics_FontSize.md) | Установка размера шрифта |
|  | [FontSpacing](P_TFlex_Drawing_Graphics_FontSpacing.md) | Установка дополнительного интервала между символами |
|  | [FontTilt](P_TFlex_Drawing_Graphics_FontTilt.md) | Установка угла наклона шрифта |
|  | [FontVerticalAlignment](P_TFlex_Drawing_Graphics_FontVerticalAlignment.md) | Установка выравнивания текста по вертикали |
|  | [IsDisplayDevice](P_TFlex_Drawing_Graphics_IsDisplayDevice.md) | Текущий вывод производится на экран |
|  | [IsExportDevice](P_TFlex_Drawing_Graphics_IsExportDevice.md) | Текущий вывод производится в файл другого формата |
|  | [IsMarkDevice](P_TFlex_Drawing_Graphics_IsMarkDevice.md) | Текущий вывод производится для пометки объекта |
|  | [IsPrinterDevice](P_TFlex_Drawing_Graphics_IsPrinterDevice.md) | Текущий вывод производится на принтер |
|  | [LCSRectangle](P_TFlex_Drawing_Graphics_LCSRectangle.md) | Прямоугольник вывода в системе координат графического устройства |
|  | [LineWidth](P_TFlex_Drawing_Graphics_LineWidth.md) | Толщина линии для функций вывода линий, полилиний, текстов и других линейных объектов |
|  | [MarkColor](P_TFlex_Drawing_Graphics_MarkColor.md) | Цвет, используемый для пометки элементов |
|  | [RGBBkColor](P_TFlex_Drawing_Graphics_RGBBkColor.md) | Цвет фона в виде компонент красного, зелёного и синего |
|  | [RGBColor](P_TFlex_Drawing_Graphics_RGBColor.md) | Цвет, которым производится вывод, в виде компонент красного, зелёного и синего |
|  | [Rop](P_TFlex_Drawing_Graphics_Rop.md) | Тип растровой операции, установленной для вывода |
|  | [Scale](P_TFlex_Drawing_Graphics_Scale.md) | Масштаб преобразования в систему координат графического устройства |
|  | [WCSRectangle](P_TFlex_Drawing_Graphics_WCSRectangle.md) | Прямоугольник вывода в мировой системе координат |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDashLine](M_TFlex_Drawing_Graphics_AddDashLine.md) | Добавление в массив штрихов штрихового типа линии сплошного штриха |
|  | [AddDashSpace](M_TFlex_Drawing_Graphics_AddDashSpace.md) | Добавление в массив штрихов штрихового типа линии пробела (интервала между штрихами) |
|  | [Arc(Point, Point, Point)](M_TFlex_Drawing_Graphics_Arc.md) | Прорисовка дуги с центром в заданной точке, проходящей через две точки, против часовой стрелки |
|  | [Arc(Point, Point, Point, Boolean)](M_TFlex_Drawing_Graphics_Arc_1.md) | Прорисовка дуги с центром в заданной точке, проходящей через две точки |
|  | [Arc3Points](M_TFlex_Drawing_Graphics_Arc3Points.md) | Прорисовка дуги, проходящей через три точки |
|  | [ArrowArc](M_TFlex_Drawing_Graphics_ArrowArc.md) | Прорисовка дуги со стрелками с центром в заданной точке, проходящей через две точки, против часовой стрелки |
|  | [ArrowLine](M_TFlex_Drawing_Graphics_ArrowLine.md) | Прорисовка отрезка со стрелками |
|  | [ArrowPolyline](M_TFlex_Drawing_Graphics_ArrowPolyline.md) | Прорисовка полилинии со стрелками |
|  | [BeginDraw](M_TFlex_Drawing_Graphics_BeginDraw.md) | Начало вывода изображения |
|  | [Circle(Point, Double)](M_TFlex_Drawing_Graphics_Circle.md) | Прорисовка окружности |
|  | [Circle(Point, Point)](M_TFlex_Drawing_Graphics_Circle_1.md) | Прорисовка окружности |
|  | [ClearBackground](M_TFlex_Drawing_Graphics_ClearBackground.md) | Очистка фона |
|  | [ClearDashes](M_TFlex_Drawing_Graphics_ClearDashes.md) | Сброс массива штрихов штрихового типа линии |
|  | [Dispose](M_TFlex_Drawing_Graphics_Dispose.md) | Выполняет определяемые приложением задачи, связанные с удалением, высвобождением или сбросом неуправляемых ресурсов |
|  | [DrawBitmap](M_TFlex_Drawing_Graphics_DrawBitmap.md) |  |
|  | [DrawMarker](M_TFlex_Drawing_Graphics_DrawMarker.md) | Вывод маркера |
|  | [DrawText](M_TFlex_Drawing_Graphics_DrawText.md) | Вывод текста в указанной точке |
|  | [EndDraw](M_TFlex_Drawing_Graphics_EndDraw.md) | Завершение вывода изображения |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Fill](M_TFlex_Drawing_Graphics_Fill.md) | Заливка области, ограниченной полилинией |
|  | [FillRectangle](M_TFlex_Drawing_Graphics_FillRectangle.md) | Заливка прямоугольника |
|  | [FillRectangleTransparent](M_TFlex_Drawing_Graphics_FillRectangleTransparent.md) |  |
|  | [GetDeviceContext](M_TFlex_Drawing_Graphics_GetDeviceContext.md) | Получение дескриптора графического устройства (HDC) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetLCSPoint](M_TFlex_Drawing_Graphics_GetLCSPoint.md) | Получение координат точки, координаты которой заданы в мировой системе координат (системе координат модели), в системе координат графического устройства |
|  | [GetLinePatternNames](M_TFlex_Drawing_Graphics_GetLinePatternNames.md) | Получение списка названий стилей линий |
|  | [GetLinePatternPreview](M_TFlex_Drawing_Graphics_GetLinePatternPreview.md) | Получение изображения для предпросмотра стиля линии |
|  | [GetLinePatterns](M_TFlex_Drawing_Graphics_GetLinePatterns.md) | Получение списка названий стилей линий |
|  | [GetTextHeight](M_TFlex_Drawing_Graphics_GetTextHeight.md) | Получение высоты текста с текущими установками шрифта |
|  | [GetTextLength](M_TFlex_Drawing_Graphics_GetTextLength.md) | Получение длины текста с текущими установками шрифта |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetWCSPoint](M_TFlex_Drawing_Graphics_GetWCSPoint.md) | Получение координат точки, координаты которой заданы в системе графического устройства, в мировой системе координат (системе координат модели) |
|  | [Line](M_TFlex_Drawing_Graphics_Line.md) | Прорисовка отрезка между двумя точками |
|  | [LineTo](M_TFlex_Drawing_Graphics_LineTo.md) | Прорисовка отрезка от указателя к данной точке |
|  | [MoveTo](M_TFlex_Drawing_Graphics_MoveTo.md) | Перемещение указателя в точку |
|  | [Polyline](M_TFlex_Drawing_Graphics_Polyline.md) | Прорисовка полилинии |
|  | [Rectangle](M_TFlex_Drawing_Graphics_Rectangle.md) | Прорисовка границ прямоугольника |
|  | [ReleaseDeviceContext](M_TFlex_Drawing_Graphics_ReleaseDeviceContext.md) | Освобождение дескриптора графического устройства (HDC) |
|  | [SetBkColor](M_TFlex_Drawing_Graphics_SetBkColor.md) | Установка цвета фона |
|  | [SetColor](M_TFlex_Drawing_Graphics_SetColor.md) | Установка цвета, которым должен производиться вывод |
|  | [SetColorLock](M_TFlex_Drawing_Graphics_SetColorLock.md) | Установка режима запрета смены цвета (одноцветный режим) |
|  | [SetDashedType](M_TFlex_Drawing_Graphics_SetDashedType.md) | Установка прорисовки шрихового типа линии |
|  | [SetEraseMode](M_TFlex_Drawing_Graphics_SetEraseMode.md) | Установка режима очистки фона |
|  | [SetFontName](M_TFlex_Drawing_Graphics_SetFontName.md) | Выбор шрифта для прорисовки текста |
|  | [SetFontRotation](M_TFlex_Drawing_Graphics_SetFontRotation.md) | Установка угла поворота текста с помощью вектора вертикали |
|  | [SetLineWidth](M_TFlex_Drawing_Graphics_SetLineWidth.md) | Установка толщины линии для функций вывода линий, полилиний, текстов и других линейных объектов |
|  | [SetRGBBkColor(Int32)](M_TFlex_Drawing_Graphics_SetRGBBkColor.md) | Установка цвета фона в виде компонент красного, зелёного и синего |
|  | [SetRGBBkColor(Int32, Int32, Int32)](M_TFlex_Drawing_Graphics_SetRGBBkColor_1.md) | Установка цвета фона в виде компонент красного, зелёного и синего |
|  | [SetRGBColor(Int32)](M_TFlex_Drawing_Graphics_SetRGBColor.md) | Установка цвета, которым должен производиться вывод, в виде компонент красного, зелёного и синего |
|  | [SetRGBColor(Int32, Int32, Int32)](M_TFlex_Drawing_Graphics_SetRGBColor_1.md) | Установка цвета, которым должен производиться вывод, в виде компонент красного, зелёного и синего |
|  | [SetRop](M_TFlex_Drawing_Graphics_SetRop.md) | Установка типа растровой операции, которую необходимо использовать для вывода |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
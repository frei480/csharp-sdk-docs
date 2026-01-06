

Руководство по T-FLEX CAD Open API

# View3DDrawStyle - структура  
    
Стиль изображения в 3D окне

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemValueType](https://learn.microsoft.com/dotnet/api/system.valuetype) TFlex.Model.Model3DView3DDrawStyle

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public struct DrawStyle
```




Тип View3DDrawStyle предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [SemitransparentMode](P_TFlex_Model_Model3D_View3D_DrawStyle_SemitransparentMode.md) | Полупрозрачный режим |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AreFaceEdgesShown](M_TFlex_Model_Model3D_View3D_DrawStyle_AreFaceEdgesShown.md) | Возвращает true в случае, когда в текущем режиме задана опция "показывать рёбра" |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.valuetype.equals) | Indicates whether this instance and a specified object are equal.(Унаследован от [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.valuetype.gethashcode) | Returns the hash code for this instance.(Унаследован от [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IsFilled](M_TFlex_Model_Model3D_View3D_DrawStyle_IsFilled.md) | Возвращает true в случае, когда задан режим тоновой закраски или тоновой закраски с материалами |
|  | [IsHiddenLine](M_TFlex_Model_Model3D_View3D_DrawStyle_IsHiddenLine.md) | Возвращает true в случае, когда задан один из режимов удаления невидимых линий |
|  | [IsWireframe](M_TFlex_Model_Model3D_View3D_DrawStyle_IsWireframe.md) | Возвращает true в случае, когда задан режим проволочной модели или удаления невидимых линий |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.valuetype.tostring) | Returns the fully qualified type name of this instance.(Унаследован от [ValueType](https://learn.microsoft.com/dotnet/api/system.valuetype)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(View3DDrawStyle, View3DDrawStyle)](M_TFlex_Model_Model3D_View3D_DrawStyle_op_Equality.md) |  |
|  | [Inequality(View3DDrawStyle, View3DDrawStyle)](M_TFlex_Model_Model3D_View3D_DrawStyle_op_Inequality.md) |  |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [CurrentStyle](F_TFlex_Model_Model3D_View3D_DrawStyle_CurrentStyle.md) | Основной стиль изображения |
|  | [HiresOptions](F_TFlex_Model_Model3D_View3D_DrawStyle_HiresOptions.md) | Дополнительные опции режима тоновой закраски с материалами |
|  | [PrecisehiddenOptions](F_TFlex_Model_Model3D_View3D_DrawStyle_PrecisehiddenOptions.md) | Дополнительные опции режима с точным удалением скрытых линий |
|  | [QuickhiddenOptions](F_TFlex_Model_Model3D_View3D_DrawStyle_QuickhiddenOptions.md) | Дополнительные опции режима с быстрым удалением скрытых линий |
|  | [ShadingOptions](F_TFlex_Model_Model3D_View3D_DrawStyle_ShadingOptions.md) | Дополнительные опции режима тоновой закраски |
|  | [WireframeOptions](F_TFlex_Model_Model3D_View3D_DrawStyle_WireframeOptions.md) | Дополнительные опции режима проволочной модели |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# Управление параметрами вывода  
    
Весь вывод графической информации класса [Graphics](T_TFlex_Drawing_Graphics.md) производится в соответствии с параметрами вывода. К таким параметрам относится цвет, толщина линий, тип растровой операции, и т.д. Ниже описаны методы управления данными параметрами, а также методы их получения.

  * Управление цветом вывода элементов: 

[SetColor](M_TFlex_Drawing_Graphics_SetColor.md) — установить цвет вывода элементов. Возвращается цвет, который был установлен до этого. 

[Color](P_TFlex_Drawing_Graphics_Color.md) — получить текущий цвет. 

  * Управление цветом вывода элементов в виде RGB: 

[SetRGBColor](Overload_TFlex_Drawing_Graphics_SetRGBColor.md) — установить цвет вывода элементов. Возвращается цвет, который был установлен до этого. 

[RGBColor](P_TFlex_Drawing_Graphics_RGBColor.md) — получить текущий цвет. 

  * Управление цветом фона: 

[SetBkColor](M_TFlex_Drawing_Graphics_SetBkColor.md) — установить цвет фона. Возвращается цвет фона, который был установлен до этого. 

[BkColor](P_TFlex_Drawing_Graphics_BkColor.md) — получить текущий цвет фона. 

  * Управление цветом фона в виде RGB: 

[SetRGBBkColor](Overload_TFlex_Drawing_Graphics_SetRGBBkColor.md) — установить цвет фона. Возвращается цвет фона, который был установлен до этого. 

[RGBBkColor](P_TFlex_Drawing_Graphics_RGBBkColor.md) — получить текущий цвет фона. 

  * Управление режимом запрета смены цвета: 

[SetColorLock](M_TFlex_Drawing_Graphics_SetColorLock.md) — установить или отменить режим запрета смены цвета. Возвращается режим, который был установлен до вызова данного метода. 

[ColorLock](P_TFlex_Drawing_Graphics_ColorLock.md) — получить режим запрета смены цвета. 

  * Управление типом растровой операции вывода: 

[SetRop](M_TFlex_Drawing_Graphics_SetRop.md) — установить текущий тип растровой операции. Возвращается предыдущий тип растровой операции. 

[Rop](P_TFlex_Drawing_Graphics_Rop.md) — получить текущий тип растровой операции. 

  * Управление толщиной линий: 

[SetLineWidth](M_TFlex_Drawing_Graphics_SetLineWidth.md) — установить текущее значений толщины линий. Возвращается предыдущее значение толщины. 

[LineWidth](P_TFlex_Drawing_Graphics_LineWidth.md) — получить текущее значений толщины линий. 




#### Другие ресурсы

[Класс Graphics. Общие положения.](fd0e70f9-6abc-42ad-896b-9ae7523ad12e.md)
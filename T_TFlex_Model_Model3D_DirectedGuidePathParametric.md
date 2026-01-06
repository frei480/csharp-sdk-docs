

Руководство по T-FLEX CAD Open API

# DirectedGuidePathParametric - класс  
    
Класс для описания системы координат копии по путям и последовательностям поверхностей

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3DParametric](T_TFlex_Model_Model3D_Parametric.md) [TFlex.Model.Model3DGuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md) TFlex.Model.Model3DDirectedGuidePathParametric

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class DirectedGuidePathParametric : GuidePathParametric
```
```vb
Public NotInheritable Class DirectedGuidePathParametric
	Inherits GuidePathParametric
```
```cpp
public ref class DirectedGuidePathParametric sealed : public GuidePathParametric
```


Тип DirectedGuidePathParametric предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [DirectedGuidePathParametric](M_TFlex_Model_Model3D_DirectedGuidePathParametric__ctor.md) | Конструктор для создания свойств параметрического объекта |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AxisX](P_TFlex_Model_Model3D_GuidePathParametric_AxisX.md) | Переменные, в которые записывается ориентация оси X системы координат(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [AxisY](P_TFlex_Model_Model3D_GuidePathParametric_AxisY.md) | Переменные, в которые записывается ориентация оси Y системы координат(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [AxisZ](P_TFlex_Model_Model3D_GuidePathParametric_AxisZ.md) | Переменные, в которые записывается ориентация оси Z системы координат(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [Direction](P_TFlex_Model_Model3D_DirectedGuidePathParametric_Direction.md) | Способ определения направления осей |
|  | [GuidePath](P_TFlex_Model_Model3D_GuidePathParametric_GuidePath.md) | Множество проволочных моделей, образующих составной путь(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [Number](P_TFlex_Model_Model3D_Parametric_Number.md) | Переменная номера копии(Унаследован от [Parametric](T_TFlex_Model_Model3D_Parametric.md)) |
|  | [OffsetFunction](P_TFlex_Model_Model3D_GuidePathParametric_OffsetFunction.md) | Функция смещения от начала пути (натуральная параметризация)(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [OffsetValue](P_TFlex_Model_Model3D_GuidePathParametric_OffsetValue.md) | Переменная, в которую записывается расcчитанное значение смещения от начала пути (натуральная параметризация)(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [Origin](P_TFlex_Model_Model3D_GuidePathParametric_Origin.md) | Переменные, в которые записывается положение системы координат(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [ParamFunction](P_TFlex_Model_Model3D_GuidePathParametric_ParamFunction.md) | Функция параметра (нормализованный параметр [0.0, 1.0])(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [ParamValue](P_TFlex_Model_Model3D_GuidePathParametric_ParamValue.md) | Переменная, в которую записывается расcчитанное значение параметра(нормализованный параметр [0.0, 1.0])(Унаследован от [GuidePathParametric](T_TFlex_Model_Model3D_GuidePathParametric.md)) |
|  | [Quantity](P_TFlex_Model_Model3D_Parametric_Quantity.md) | Количество копий(Унаследован от [Parametric](T_TFlex_Model_Model3D_Parametric.md)) |
|  | [SourceLCS](P_TFlex_Model_Model3D_Parametric_SourceLCS.md) | Исходная система координат(Унаследован от [Parametric](T_TFlex_Model_Model3D_Parametric.md)) |
|  | [XPath](P_TFlex_Model_Model3D_DirectedGuidePathParametric_XPath.md) | Множество проволочных моделей, образующих составной путь для определения направления оси X |
|  | [XSurface](P_TFlex_Model_Model3D_DirectedGuidePathParametric_XSurface.md) | Последовательность поверхностей, определяющих направление оси X |
|  | [YPath](P_TFlex_Model_Model3D_DirectedGuidePathParametric_YPath.md) | Множество проволочных моделей, образующих составной путь для определения направления оси Y |
|  | [YSurface](P_TFlex_Model_Model3D_DirectedGuidePathParametric_YSurface.md) | Последовательность поверхностей, определяющих направление оси Y |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Форма и положение копий в параметрическом объекте задаётся несколькими путями и последовательностями поверхностей. Один путь определяет начало локальной системы координат. Положение начала системы координат задаётся параметром (нормализованный параметр [0.0, 1.0]) или смещением от начала пути (натуральная параметризация). Параметр, как правило, задаётся функцией от переменной номера копии. Направление оси X задаётся одним из двух способов: путём (касательная к пути в точке) или последовательностью поверхностей (нормаль к поверхности в точке). Направление оси Y задаётся одним из двух способов: путём (касательная к пути в точке) или последовательностью поверхностей (нормаль к поверхности в точке). Ось Z определяется как векторное произведение осей X и Y. Если ось Z не задана, то ось Z совпадает с касательной к первому пути в точке. Ось Y в этом случае определяется как вектороное произведение осей Z и X. Пересчёт выполняется в несколько этапов: 

  * определяется локальная система координат;
  * координаты локальной системы координат передаются в переменные, от которых может зависеть форма копируемого объекта;
  * пересчитывается объект;
  * к полученному результату применяется преобразование из системы координат для первой копии или ЛСК (если задана) в систему координат для текущей копии. Таким образом, первый элемент массива остаётся на месте



#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
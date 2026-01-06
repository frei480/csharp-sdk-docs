

Руководство по T-FLEX CAD Open API

# ObjectType - перечисление  
    
Тип объекта модели

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum ObjectType
```
```vb
Public Enumeration ObjectType
```
```cpp
public enum class ObjectType
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Undefined | 0 | Неопределённый тип |
| Construction | 1 | Линия построения |
| Node | 2 | Узел |
| Outline | 3 | Линия изображения |
| Dimension | 4 | Размер |
| Text | 5 | Текст |
| Layer | 7 | Слой |
| Variable | 8 | Переменная |
| Area | 9 | Штриховка или заливка |
| FormlimitsSymbol | 11 | Обозначение допуска формы или расположения |
| Fragment | 13 | Фрагмент |
| RoughnessSymbol | 14 | Обозначение шероховатости |
| LeaderNote | 15 | Надпись |
| Simplification | 16 | Операция удаления лишних геометрических элементов упрощения геометрии |
| Report | 17 | Отчёт |
| Database | 18 | База данных |
| External | 19 | Объект приложения |
| FixingVector | 20 | Вектор привязки |
| DrawingView | 21 | Чертёжный вид |
| Loop | 22 | Цикл |
| Vertex | 23 | Вершина |
| Edge | 24 | Ребро |
| Face | 25 | Грань |
| Workplane | 27 | Рабочая плоскость |
| Profile | 28 | 3D профиль |
| Operation | 29 | 3D операция |
| GraphLaw | 32 | График |
| Page | 33 | Страница |
| Mate | 39 | Сопряжение |
| Picture | 40 | Картинка или OLE объект |
| Sensor | 41 | Датчик |
| Extrusion | 42 | Операция выталкивания |
| Rotation | 43 | Операция вращения |
| Swept | 45 | Операция по траектории |
| Loft | 47 | Операция по сечениям |
| Boolean | 48 | Булева операция |
| EdgeBlending | 49 | Операция сглаживания рёбер |
| Section | 53 | 3D сечение |
| Material | 54 | Материал |
| Light | 57 | Источник света |
| CutOperation | 60 | Операция отсечения |
| NodeArray | 62 | Массив по точкам (3D) |
| Camera | 63 | Камера |
| Control | 68 | Элемент управления |
| PathArray | 69 | Массив по пути (3D) |
| Path3D | 70 | 3D путь |
| Copy | 72 | Операция копирования или массив (2D) |
| Taper | 73 | Операция уклона |
| ViewSymbol | 74 | Обозначение вида |
| Spring | 75 | Операция "пружина" |
| SpatialSurface | 77 | Рабочая поверхность |
| SpatialWorkSurface | 77 | Базовый класс для всех типов специальных координатных поверхностей |
| ParametricArray | 81 | Параметрический массив (3D) |
| LinearArray | 83 | Линейный массив (3D) |
| CircularArray | 84 | Круговой массив (3D) |
| ExtendSurface | 87 | Заполнения области |
| ImportedTransformation | 89 | Класс внешнего преобразования |
| CAEStudy | 96 | Задача КЭА |
| WorkSurface | 97 | Рабочая поверхность |
| DynamicStudy | 98 | Задача Динамического анализа |
| CircuitLinkSymbol | 100 | Условное обозначение линии связи |
| Node3D | 107 | 3D узел |
| LCS | 108 | ЛСК |
| CopyOperation | 111 | Операция копирования (3D) в T-Flex CAD до версии 11 |
| ImportedOperation | 116 | Операция импорта |
| Picture3D | 117 | 3D картинка |
| Projection | 119 | 2D проекция |
| FaceDelete | 120 | Операция удаления граней |
| FaceReplace | 121 | Операция замены граней |
| FaceChange | 122 | Операция изменения граней |
| FaceTransform | 123 | Операция перемещения граней |
| Weld3D | 126 | 3D-сварной шов |
| Weld | 129 | Сварной шов |
| WeldType | 130 | Тип сварного шва |
| Model3DObjectGroup | 131 | Группа объектов 3D модели. |
| Connector | 142 | Коннектор |
| PipePath3D | 143 | Класс пути трубопровода |
| EventFatigue | 148 | Событие |
| Harness3D | 151 | Класс пути трубопровода |
| CopyOperation2 | 157 | Операция копирования (3D) |
| SymmetryOperation2 | 159 | Операция симметрии |
| SymmetryOperation | 160 | Операция симметрии в T-Flex CAD до версии 11 |
| SketchConstraint | 163 | Ограничение эскиза |
| Topol | 174 | Топологический элемент: грань, цикл, ребро, вершина |
| MaterialOperation | 175 | Операция наложения материала |
| Shell | 176 | Операция оболочки |
| ReferenceNode3D | 178 | Внешний 3D узел |
| FaceBlending | 184 | Операция сглаживания граней |
| ThreeFaceBlending | 187 | Операция сглаживания трёх граней |
| RotateVectorTransformation | 189 | Класс преобразования поворота вокруг вектора |
| BodyTaper | 190 | Операция уклона тела |
| SheetMetalPart | 193 | Заготовка листовой штамповки |
| InternalFragment3D | 194 | Внутренний 3D фрагмент |
| MoveVectorTransformation | 195 | Класс преобразования перемещения вдоль вектора |
| ScaleVectorTransformation | 196 | Класс преобразования масштабирования вдоль вектора |
| SheetMetalFeature | 197 | Операция выштамповки |
| Imprint | 199 | Операция разделения граней |
| ExternalOperation | 201 | Внешняя операция (приложения) |
| Hole | 204 | Операция отверстия |
| Bend | 206 | Операция гибки |
| Pipe | 209 | Операциия трубопровода |
| Primitive | 211 | 3D Примитив |
| Fragment3D | 214 | 3D фрагмент |
| ReferenceWorkplane | 223 | Ссылочная рабочая плоскость |
| Sew | 227 | Операция сшивки |
| Unbend | 231 | Операция разгибки |
| Rebend | 232 | Операция повторной гибки |
| MoveRotateTransformation | 237 | Класс преобразования перемещения/поворота |
| FillHole | 238 | Заполнения области |
| Restraint | 240 | Граничное условие задачи |
| Thread | 247 | Операция резьбы |
| Spiral | 250 | Операция "спираль" |
| Separation | 253 | Операция разделения |
| ProductStructRowElem | 264 | Элемент состава изделия |
| ProductStruct | 265 | Состав изделия |
| Scenario | 266 | Сценарий разборки |
| StructureElementType | 269 | Тип структурного элемента |
| StructureElement | 270 | Структурный элемент |
| StructureElementLinkDescriptor | 271 | Описание связи структурных элементов |
| StructureElementLink | 272 | Связь структурных элементов |
| Body | 273 | Тело |
| CircuitLink | 277 | Линия связи |
| CircuitLinksGroup | 278 | Групповая линия связи |
| CircuitMultiLink | 282 | Линия связи с разрывом |
| CircuitMultiLinksGroup | 283 | Групповая линия связи с разрывом |
| Harness2D | 297 | Жгут 2D (cборочный чертёж кабельного изделия) |
| CircuitBus | 305 | Шина |
| MeshNode3D | 591 | 3D узел |
| TwoPathesIntersectionNode3D | 600 | 3D узел |
| RealNode3D | 700 |  |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
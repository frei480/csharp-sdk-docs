

Руководство по T-FLEX CAD Open API

# ArrowProjection - класс  
    
Класс создания проекции по стрелке

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.ModelModelObject](T_TFlex_Model_ModelObject.md) [TFlex.Model.Model3DObject3D](T_TFlex_Model_Model3D_Object3D.md) [TFlex.Model.Model3DProjection](T_TFlex_Model_Model3D_Projection.md) [TFlex.Model.Model3DSimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md) TFlex.Model.Model3DArrowProjection

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public class ArrowProjection : SimpleDrawingProjection
```




Тип ArrowProjection предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ArrowProjection(Document)](M_TFlex_Model_Model3D_ArrowProjection__ctor.md) | Конструктор для создания новой проекции |
|  | [ArrowProjection(Document, Page)](M_TFlex_Model_Model3D_ArrowProjection__ctor_1.md) | Конструктор для создания новой проекции |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Angle](P_TFlex_Model_Model3D_Projection_Angle.md) | Угол поворота проекции(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [Arrow](P_TFlex_Model_Model3D_ArrowProjection_Arrow.md) | Стрелка взгляда |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Auxiliary](P_TFlex_Model_Model3D_Object3D_Auxiliary.md) | Внутрисистемный объект. Используется для Refer объектов фрагментов. Такие объекты скрыты от пользователя. Работа с такими объектами может быть реализована на уровне API.NET или ядром TFlex. Такие объекты не передаются на следующий уровень сборки. (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [AxisCreate](P_TFlex_Model_Model3D_SimpleDrawingProjection_AxisCreate.md) | Признак режима создания осей(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [AxisLineColor](P_TFlex_Model_Model3D_SimpleDrawingProjection_AxisLineColor.md) | Цвет осевых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [AxisLineName](P_TFlex_Model_Model3D_SimpleDrawingProjection_AxisLineName.md) | Имя типа осевых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [AxisLineScale](P_TFlex_Model_Model3D_SimpleDrawingProjection_AxisLineScale.md) | Масштаб осевых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [AxisLineWidth](P_TFlex_Model_Model3D_SimpleDrawingProjection_AxisLineWidth.md) | Толщина осевых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [BaseProjection](P_TFlex_Model_Model3D_ArrowProjection_BaseProjection.md) | Проекция на которой расположена стрелка взгляда |
|  | [Bind](P_TFlex_Model_Model3D_Projection_Bind.md) | Проекция с которой берётся проекционная связь(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BoundRect](P_TFlex_Model_Model3D_Projection_BoundRect.md) | Ограничивающий прямоугольник проекции(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenAmplitude](P_TFlex_Model_Model3D_Projection_BrokenAmplitude.md) | Амплитуда линии разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenAngle](P_TFlex_Model_Model3D_Projection_BrokenAngle.md) | Угол поворота набора линий разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenBorder](P_TFlex_Model_Model3D_Projection_BrokenBorder.md) | Длина выносной линии(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenHAlign](P_TFlex_Model_Model3D_Projection_BrokenHAlign.md) | Тип горизонтального выравнивания(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenLength](P_TFlex_Model_Model3D_Projection_BrokenLength.md) | Длина полупериода волны линии разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenLineColor](P_TFlex_Model_Model3D_Projection_BrokenLineColor.md) | Цвет линий разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenLineDistance](P_TFlex_Model_Model3D_Projection_BrokenLineDistance.md) | Расстояние между линиями разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenLineName](P_TFlex_Model_Model3D_Projection_BrokenLineName.md) | Имя типа линий разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenLineScale](P_TFlex_Model_Model3D_Projection_BrokenLineScale.md) | Масштаб линий разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenLineWidth](P_TFlex_Model_Model3D_Projection_BrokenLineWidth.md) | Толщина линий разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenMetric](P_TFlex_Model_Model3D_Projection_BrokenMetric.md) | Единицы измерения величины разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenType](P_TFlex_Model_Model3D_Projection_BrokenType.md) | Тип линии разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [BrokenVAlign](P_TFlex_Model_Model3D_Projection_BrokenVAlign.md) | Тип вертикального выравнивания(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [Color](P_TFlex_Model_Model3D_Object3D_Color.md) | Цвет(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ConstTransformations](P_TFlex_Model_Model3D_Object3D_ConstTransformations.md) | **Устарело.** Преобразование 3D объекта для чтения (устаревшая версия трансформации - допускается чтение трансформации в старых документах.)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ConvertPolylinesToSplines](P_TFlex_Model_Model3D_SimpleDrawingProjection_ConvertPolylinesToSplines.md) | Признак режима конвертации полилиний в сплайны(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [CreateHidden](P_TFlex_Model_Model3D_SimpleDrawingProjection_CreateHidden.md) | Признак режима создания изображений с невидимыми линиями(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [CreateSection](P_TFlex_Model_Model3D_SimpleDrawingProjection_CreateSection.md) | Признак режима создания изображений с линиями сечений(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [CreateTangentEdges](P_TFlex_Model_Model3D_SimpleDrawingProjection_CreateTangentEdges.md) | Режим создания изображений с показом гладких сопряжений(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [CreateThreads](P_TFlex_Model_Model3D_SimpleDrawingProjection_CreateThreads.md) | Признак режима создания изображений резьб(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Explode](P_TFlex_Model_Model3D_SimpleDrawingProjection_Explode.md) | Признак режима разборки(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [FileLink](P_TFlex_Model_Model3D_Projection_FileLink.md) | Ссылка на файл, из которого берутся проецируемые элементы(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [GroupType](P_TFlex_Model_Model3D_Projection_GroupType.md) | Тип объекта(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [HiddenLineColor](P_TFlex_Model_Model3D_SimpleDrawingProjection_HiddenLineColor.md) | Цвет невидимых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [HiddenLineWidth](P_TFlex_Model_Model3D_SimpleDrawingProjection_HiddenLineWidth.md) | Толщина невидимых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [InScene](P_TFlex_Model_Model3D_Object3D_InScene.md) | Объект в сцене(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model3D_Object3D_Layer.md) | Слой, на котором размещается объект(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Layers](P_TFlex_Model_Model3D_Projection_Layers.md) | Множество слоёв(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [LayersFilter](P_TFlex_Model_Model3D_Projection_LayersFilter.md) | (Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [Level](P_TFlex_Model_Model3D_Object3D_Level.md) | Уровень(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Monochrome](P_TFlex_Model_Model3D_SimpleDrawingProjection_Monochrome.md) | Признак использования одного цвета на всей проекции(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OverlapBodies](P_TFlex_Model_Model3D_SimpleDrawingProjection_OverlapBodies.md) | Режим учёта перекрытия тел при проецировании(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [Page](P_TFlex_Model_Model3D_Projection_Page.md) | Страница, где отображается проекция(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Perspective](P_TFlex_Model_Model3D_SimpleDrawingProjection_Perspective.md) | Перспективная проекция(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [ProjectionClass](P_TFlex_Model_Model3D_SimpleDrawingProjection_ProjectionClass.md) | Тип проекции(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [ProjectPrecision](P_TFlex_Model_Model3D_SimpleDrawingProjection_ProjectPrecision.md) | Получить значение точности проецирования(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [RecognizeCircles](P_TFlex_Model_Model3D_SimpleDrawingProjection_RecognizeCircles.md) | Признак режима распознавания дуг окружностей(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [RecognizeLines](P_TFlex_Model_Model3D_SimpleDrawingProjection_RecognizeLines.md) | Признак режима распознавания отрезков(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [RegenerationMode](P_TFlex_Model_Model3D_SimpleDrawingProjection_RegenerationMode.md) | Режим регенерации проекции(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [Save3DDim](P_TFlex_Model_Model3D_Projection_Save3DDim.md) | Сохранять информацию для 3D размеров(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [Scale](P_TFlex_Model_Model3D_Projection_Scale.md) | Масштаб проекции(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SmoothLineColor](P_TFlex_Model_Model3D_SimpleDrawingProjection_SmoothLineColor.md) | Цвет линий гладких сопряжений(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [SmoothLineName](P_TFlex_Model_Model3D_SimpleDrawingProjection_SmoothLineName.md) | Имя типа видимых линий гладких сопряжений(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [SmoothLineScale](P_TFlex_Model_Model3D_SimpleDrawingProjection_SmoothLineScale.md) | Масштаб линий гладких сопряжений(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [SmoothLineWidth](P_TFlex_Model_Model3D_SimpleDrawingProjection_SmoothLineWidth.md) | Толщина линий гладких сопряжений(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [SourcePage](P_TFlex_Model_Model3D_Projection_SourcePage.md) | Исходная страница проекции(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [ThreadLineColor](P_TFlex_Model_Model3D_SimpleDrawingProjection_ThreadLineColor.md) | Цвет линий резьбы(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [ThreadLineName](P_TFlex_Model_Model3D_SimpleDrawingProjection_ThreadLineName.md) | Имя типа линий резьбы(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [ThreadLineScale](P_TFlex_Model_Model3D_SimpleDrawingProjection_ThreadLineScale.md) | Масштаб линий резьбы(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [ThreadLineWidth](P_TFlex_Model_Model3D_SimpleDrawingProjection_ThreadLineWidth.md) | Толщина линий резьбы(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [Transformations](P_TFlex_Model_Model3D_Object3D_Transformations.md) | Контейнер групп преобразований 3D объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [VisibleInScene](P_TFlex_Model_Model3D_Object3D_VisibleInScene.md) | Свойство видимости объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [VisibleLineColor](P_TFlex_Model_Model3D_SimpleDrawingProjection_VisibleLineColor.md) | Цвет видимых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [VisibleLineName](P_TFlex_Model_Model3D_SimpleDrawingProjection_VisibleLineName.md) | Имя типа видимых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [VisibleLineScale](P_TFlex_Model_Model3D_SimpleDrawingProjection_VisibleLineScale.md) | Масштаб видимых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [VisibleLineWidth](P_TFlex_Model_Model3D_SimpleDrawingProjection_VisibleLineWidth.md) | Толщина видимых линий(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [VolatileTransformations](P_TFlex_Model_Model3D_Object3D_VolatileTransformations.md) | **Устарело.** Преобразование 3D объекта для изменения(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddBody](M_TFlex_Model_Model3D_SimpleDrawingProjection_AddBody.md) | Добавить операцию как тело для проецирования(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [AddBreak](M_TFlex_Model_Model3D_Projection_AddBreak.md) | Метод для добавления информации о новом разрыве в список(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [AddOperation](M_TFlex_Model_Model3D_SimpleDrawingProjection_AddOperation.md) | Добавить операцию для проецирования(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [AddSection](M_TFlex_Model_Model3D_Projection_AddSection.md) | (Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [CancelRollback](M_TFlex_Model_Model3D_Object3D_CancelRollback.md) | Завершить откат(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Clone](M_TFlex_Model_Model3D_Object3D_Clone.md) | Класс для передачи ссылки на геометрические свойства родительского объекта или на отдельные геометрические элементы тел модели (грани, циклы, рёбра, вершины)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CompareTo](M_TFlex_Model_ModelObject_CompareTo.md) | Сравнение объектов по идентификаторам(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Complete](M_TFlex_Model_Model3D_Projection_Complete.md) | Для внутреннего использования(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [CopyProperties](M_TFlex_Model_ModelObject_CopyProperties.md) | Копировать свойства в буфер(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateLegacy](M_TFlex_Model_Model3D_ArrowProjection_CreateLegacy.md) |  |
|  | [CreateReference](M_TFlex_Model_Model3D_Object3D_CreateReference.md) | Создаёт ссылочный элемент в исходном документе(внутренняя ссылка)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateReference(Document)](M_TFlex_Model_Model3D_Object3D_CreateReference_1.md) | Создаёт ссылочный элемент в указанном документе(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CreateStyle(IntPtr)](M_TFlex_Model_ModelObject_CreateStyle.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [CreateStyle(IntPtr, IntPtr)](M_TFlex_Model_ModelObject_CreateStyle_1.md) | Для внутреннего использования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DeleteAllBreaks](M_TFlex_Model_Model3D_Projection_DeleteAllBreaks.md) | Удаление всех разрывов(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [DeleteBreak](M_TFlex_Model_Model3D_Projection_DeleteBreak.md) | Удаление разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [DependsOn(ListModelObject)](M_TFlex_Model_ModelObject_DependsOn.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [DependsOn(ModelObject)](M_TFlex_Model_ModelObject_DependsOn_1.md) | Проверка зависимости объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Explode](M_TFlex_Model_Model3D_Projection_Explode.md) | Разрушить проекцию(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [FromFile](M_TFlex_Model_Model3D_Projection_FromFile.md) | Создание проекции из файла(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [GetAttributes](M_TFlex_Model_ModelObject_GetAttributes.md) | Контейнер атрибутов объекта. Приложение может использовать данный контейнер для хранения своих данных, связанных с объектом(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetBrokenSize](M_TFlex_Model_Model3D_Projection_GetBrokenSize.md) | Метод для получения размера массива разрывов(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [GetEdgeMode](M_TFlex_Model_Model3D_SimpleDrawingProjection_GetEdgeMode.md) | Опрос режима отрисовки рёбер в растровых проекциях(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [GetFileLinkReference(Int32)](M_TFlex_Model_ModelObject_GetFileLinkReference.md) | Получить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetFileLinkReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_GetFileLinkReference_1.md) | Получить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetGeomReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetGeomReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetGeomReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_GetGeomReference_1.md) | Получить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetIntProp](M_TFlex_Model_ModelObject_GetIntProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetIntProperty](M_TFlex_Model_ModelObject_GetIntProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetName](M_TFlex_Model_ModelObject_GetName.md) | Получить имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetOutlineMode](M_TFlex_Model_Model3D_SimpleDrawingProjection_GetOutlineMode.md) | Опрос режима отрисовки очерка в растровых проекциях(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [GetProjectedPoint](M_TFlex_Model_Model3D_Projection_GetProjectedPoint.md) | Функция возвращает 3D точку по точке на проекции(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [GetProjectionTransform](M_TFlex_Model_Model3D_Projection_GetProjectionTransform.md) | Функция возвращает матрицу преобразования точки в 3d пространстве в систему координат проекции(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [GetProperties](M_TFlex_Model_ModelObject_GetProperties.md) | Получить описание свойств элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealProp](M_TFlex_Model_ModelObject_GetRealProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealProperty](M_TFlex_Model_ModelObject_GetRealProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRealPropertyWithUnit](M_TFlex_Model_ModelObject_GetRealPropertyWithUnit.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetReference(Int32)](M_TFlex_Model_Model3D_Object3D_GetReference.md) | Получить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetReference(Int32, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_GetReference_1.md) | Получить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetReferences](M_TFlex_Model_ModelObject_GetReferences.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRegenerationResult](M_TFlex_Model_ModelObject_GetRegenerationResult.md) | Результат пересчета объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelation](M_TFlex_Model_ModelObject_GetRelation.md) | Измерить отношение двух объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetRelationWithUnit](M_TFlex_Model_ModelObject_GetRelationWithUnit.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProp](M_TFlex_Model_ModelObject_GetTextProp.md) | **Устарело.** Измеримые свойства объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTextProperty](M_TFlex_Model_ModelObject_GetTextProperty.md) | Получить значение свойства элемента(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [GetTransformationMatrix](M_TFlex_Model_Model3D_Object3D_GetTransformationMatrix.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetViewPoint](M_TFlex_Model_Model3D_Projection_GetViewPoint.md) | Опросить координаты точки проецирования(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [InternalRegenerate](M_TFlex_Model_Model3D_Object3D_InternalRegenerate.md) | (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsKindOf](M_TFlex_Model_ModelObject_IsKindOf.md) | Проверить принадлежность объекта указанному типу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsTemporaryObject](M_TFlex_Model_ModelObject_IsTemporaryObject.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MarkChanged](M_TFlex_Model_ModelObject_MarkChanged.md) | Пометить объект как изменённый(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [OnCancelChanges](M_TFlex_Model_ModelObject_OnCancelChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [OnEndChanges](M_TFlex_Model_ModelObject_OnEndChanges.md) | (Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PasteProperties](M_TFlex_Model_ModelObject_PasteProperties.md) | Вставить свойства из буфера(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [ProjectPoint](M_TFlex_Model_Model3D_Projection_ProjectPoint.md) | Функция проецирует данную точку на проекцию(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [Regenerate](M_TFlex_Model_Model3D_Projection_Regenerate.md) | Пометить объект как изменённый(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [RemoveAllOperations](M_TFlex_Model_Model3D_SimpleDrawingProjection_RemoveAllOperations.md) | Сбросить все проецируемые операции(Унаследован от [SimpleDrawingProjection](T_TFlex_Model_Model3D_SimpleDrawingProjection.md)) |
|  | [RemoveAllSections](M_TFlex_Model_Model3D_Projection_RemoveAllSections.md) | (Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [Replace](M_TFlex_Model_ModelObject_Replace.md) | Заменить объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [RollbackToParents](M_TFlex_Model_Model3D_Object3D_RollbackToParents.md) | Откат модели к состоянию, когда из сцены выгружены потомки объекта и он сам(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ScaleFitToPageSize](M_TFlex_Model_Model3D_Projection_ScaleFitToPageSize.md) | Подбор масшатаба для проекции, чтобы умещаться на странице(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetBegin](M_TFlex_Model_Model3D_Projection_SetBegin.md) | Установка начального отступа разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetConfiguration](M_TFlex_Model_Model3D_Projection_SetConfiguration.md) | Установить имя конфигурации(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetEnd](M_TFlex_Model_Model3D_Projection_SetEnd.md) | Установка конечного отступа разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetFileLinkReference(Int32, FileLink)](M_TFlex_Model_ModelObject_SetFileLinkReference.md) | Установить ссылку на файл по ключу(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices)](M_TFlex_Model_ModelObject_SetFileLinkReference_1.md) | Установить ссылку на файл по ключу и индексу. Используется для организации массивов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference)](M_TFlex_Model_Model3D_Object3D_SetGeomReference.md) | Установить ссылку на родительский объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetGeomReference(Int32, Object3DGeomReference, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_SetGeomReference_1.md) | Установить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetLatestAlgorithmVersion](M_TFlex_Model_Model3D_Projection_SetLatestAlgorithmVersion.md) | (Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetNormal](M_TFlex_Model_Model3D_Projection_SetNormal.md) | Установка ориентации разрыва(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetProjectionsElementsType](M_TFlex_Model_Model3D_Projection_SetProjectionsElementsType.md) | (Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetReference(Int32, ModelObjectReference)](M_TFlex_Model_Model3D_Object3D_SetReference.md) | Установить ссылку на родительcкий объект по ключу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetReference(Int32, ModelObjectReference, ModelObjectArrayIndices)](M_TFlex_Model_Model3D_Object3D_SetReference_1.md) | Установить ссылку на родительский объект по ключу и индексу(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetTieNode](M_TFlex_Model_Model3D_Projection_SetTieNode.md) | Установить привязку проекции в соответствующий узел страницы(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetTiePoint](M_TFlex_Model_Model3D_Projection_SetTiePoint.md) | Установить привязку проекции в соответствующую точку страницы(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetUniqueName](M_TFlex_Model_Model3D_Object3D_SetUniqueName.md) | Установить новое уникальное имя с заданным префиксом(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [SetViewType](M_TFlex_Model_Model3D_Projection_SetViewType.md) | Установить направление проецирования для стандартных видов(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [SetViewWorkplane](M_TFlex_Model_Model3D_Projection_SetViewWorkplane.md) | Установить направление проецирования как нормаль к рабочей плоскости(Унаследован от [Projection](T_TFlex_Model_Model3D_Projection.md)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_AddMultilineText.md) | Аггрегировать новый многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineText.md) | Получить аггрегированный многострочный текст(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextBounds](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextBounds.md) | Получить габариты аггрегированного многострочного текста(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [GetMultilineTextsCount](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_GetMultilineTextsCount.md) | Количество аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [RemoveMultilineText](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_RemoveMultilineText.md) | Удалить многострочный текст по индексу(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
|  | [UpdateMultilineTextPage](M_TFlex_Model_Model2D_AggregateMultilineTextExtension_UpdateMultilineTextPage.md) | Обновить страницу аггрегированных многострочных текстов(Определяется [AggregateMultilineTextExtension](T_TFlex_Model_Model2D_AggregateMultilineTextExtension.md)) |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
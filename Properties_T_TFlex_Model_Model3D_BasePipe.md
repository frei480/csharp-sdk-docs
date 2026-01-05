

Руководство по T-FLEX CAD Open API

# BasePipe - свойства  
  
---  
  
Тип [BasePipe](T_TFlex_Model_Model3D_BasePipe.md) предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Accuracy](P_TFlex_Model_Model3D_BasePipe_Accuracy.md) | Точность геометрии |
|  | [Attributes](P_TFlex_Model_ModelObject_Attributes.md) | **Устарело.**(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Auxiliary](P_TFlex_Model_Model3D_Object3D_Auxiliary.md) | Внутрисистемный объект. Используется для Refer объектов фрагментов. Такие объекты скрыты от пользователя. Работа с такими объектами может быть реализована на уровне API.NET или ядром TFlex. Такие объекты не передаются на следующий уровень сборки. (Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [BaseProfileProps](P_TFlex_Model_Model3D_BasePipe_BaseProfileProps.md) |  |
|  | [BeginBorder](P_TFlex_Model_Model3D_BasePipe_BeginBorder.md) | Начальная граница трубопровода |
|  | [BeginPart](P_TFlex_Model_Model3D_BasePipe_BeginPart.md) | Специальное "окончание" трубы |
|  | [Body](P_TFlex_Model_Model3D_Operation_Body.md) | Тело, в которое входит операция(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [CoatingMaterial](P_TFlex_Model_Model3D_Operation_CoatingMaterial.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Color](P_TFlex_Model_Model3D_Object3D_Color.md) | Цвет(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [ConstTransformations](P_TFlex_Model_Model3D_Object3D_ConstTransformations.md) | **Устарело.** Преобразование 3D объекта для чтения (устаревшая версия трансформации - допускается чтение трансформации в старых документах.)(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [CountCuttingItem](P_TFlex_Model_Model3D_BasePipe_CountCuttingItem.md) | Количество операций "врезки" |
|  | [DisplayName](P_TFlex_Model_ModelObject_DisplayName.md) | Отображаемое название объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Document](P_TFlex_Model_ModelObject_Document.md) | Документ, являющийся родительским для данного объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Editable](P_TFlex_Model_ModelObject_Editable.md) | Объект находится в состоянии редактирования(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [EndBorder](P_TFlex_Model_Model3D_BasePipe_EndBorder.md) | Конечная граница трубопровода |
|  | [EndPart](P_TFlex_Model_Model3D_BasePipe_EndPart.md) | Специальное "окончание" трубы |
|  | [Facet](P_TFlex_Model_Model3D_Operation_Facet.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Fixed](P_TFlex_Model_Model3D_Operation_Fixed.md) | Свойство фиксации операции относительно сопряжений(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Geometry](P_TFlex_Model_Model3D_Operation_Geometry.md) | Геометрические данные операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [GroupType](P_TFlex_Model_Model3D_BasePipe_GroupType.md) | (Переопределяет [OperationGroupType](P_TFlex_Model_Model3D_Operation_GroupType.md)) |
|  | [ID](P_TFlex_Model_ModelObject_ID.md) | **Устарело.** Идентификатор объекта. Идентификатор является уникальным числом для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [InScene](P_TFlex_Model_Model3D_Object3D_InScene.md) | Объект в сцене(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [IsDisposed](P_TFlex_Model_ModelObject_IsDisposed.md) | Объект удален из модели(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsInModelObjectGroup](P_TFlex_Model_ModelObject_IsInModelObjectGroup.md) | Является ли объект элементом группы(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [IsRevers](P_TFlex_Model_Model3D_BasePipe_IsRevers.md) | Возвращает true, если направление трубы (от начальной к конечной границе) не совпадает с направлением пути |
|  | [IsSetBeginPart](P_TFlex_Model_Model3D_BasePipe_IsSetBeginPart.md) | Наличие специального "окончания" трубы, как фрагмента |
|  | [IsSetEndPart](P_TFlex_Model_Model3D_BasePipe_IsSetEndPart.md) | Наличие специального "окончания" трубы, как фрагмента |
|  | [IsSetMidPart](P_TFlex_Model_Model3D_BasePipe_IsSetMidPart.md) | Наличие специальной "середины" трубы, как адаптивный фрагмент |
|  | [IsTransparencyOn](P_TFlex_Model_Model3D_Operation_IsTransparencyOn.md) | Управление прозрачностью(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [IsVisible](P_TFlex_Model_ModelObject_IsVisible.md) | **Устарело.** Это свойство устарело и будет удалено. Пожалуйста, используйте свойство 'Visible'.(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Layer](P_TFlex_Model_Model3D_Object3D_Layer.md) | Слой, на котором размещается объект(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Level](P_TFlex_Model_Model3D_Object3D_Level.md) | Уровень(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Material](P_TFlex_Model_Model3D_Operation_Material.md) | Материал операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MaterialDistributionLaw](P_TFlex_Model_Model3D_Operation_MaterialDistributionLaw.md) | (Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MeshDensity](P_TFlex_Model_Model3D_Operation_MeshDensity.md) | Плотность сетки в диапазоне 0.0-1.0(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [MidPart](P_TFlex_Model_Model3D_BasePipe_MidPart.md) | Специальная "середина" трубы |
|  | [ModelObjectGroup](P_TFlex_Model_ModelObject_ModelObjectGroup.md) | Группа, которая включает данный объект(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Name](P_TFlex_Model_ModelObject_Name.md) | Имя объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [NotCreateSolids](P_TFlex_Model_Model3D_BasePipe_NotCreateSolids.md) | Не создавать твёрдотельную геометрию |
|  | [ObjectId](P_TFlex_Model_ModelObject_ObjectId.md) | Идентификатор объекта. Идентификатор является уникальным для каждого из объектов одного документа(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [PageScale](P_TFlex_Model_ModelObject_PageScale.md) | Масштаб страницы объекта(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Parents](P_TFlex_Model_ModelObject_Parents.md) | Контейнер родительских объектов(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [Path](P_TFlex_Model_Model3D_BasePipe_Path.md) | Путь, используется вместо Wires |
|  | [PipeSegments](P_TFlex_Model_Model3D_BasePipe_PipeSegments.md) | **Устарело.** Возвращает информацию об участках трубопровода |
|  | [Simplify](P_TFlex_Model_Model3D_BasePipe_Simplify.md) | Параметр упрощения геометрии |
|  | [Suppression](P_TFlex_Model_Model3D_Operation_Suppression.md) | Свойство подавленности операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [TopLevel](P_TFlex_Model_Model3D_Operation_TopLevel.md) | Признак верхней операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [TopOperation](P_TFlex_Model_Model3D_Operation_TopOperation.md) | Верхняя операция в теле(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Transformations](P_TFlex_Model_Model3D_Object3D_Transformations.md) | Контейнер групп преобразований 3D объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Transparency](P_TFlex_Model_Model3D_Operation_Transparency.md) | Прозрачность(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Visible](P_TFlex_Model_ModelObject_Visible.md) | Является ли объект видимым(Унаследован от [ModelObject](T_TFlex_Model_ModelObject.md)) |
|  | [VisibleInScene](P_TFlex_Model_Model3D_Object3D_VisibleInScene.md) | Свойство видимости объекта(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [VolatileTransformations](P_TFlex_Model_Model3D_Object3D_VolatileTransformations.md) | **Устарело.** Преобразование 3D объекта для изменения(Унаследован от [Object3D](T_TFlex_Model_Model3D_Object3D.md)) |
|  | [Wireframe](P_TFlex_Model_Model3D_Operation_Wireframe.md) | Признак рёберной отрисовки операции(Унаследован от [Operation](T_TFlex_Model_Model3D_Operation.md)) |
|  | [Wires](P_TFlex_Model_Model3D_BasePipe_Wires.md) | Путь трубопровода |
  
#### Ссылки

[BasePipe - ](T_TFlex_Model_Model3D_BasePipe.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
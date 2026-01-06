# Продвинутые примеры использования классов в пространстве имён TFlex.Model.Model3D

## Комплексные сценарии работы с 3D-моделями

### Создание сложной трансформации с несколькими операциями

```csharp
public void CreateComplexTransformation(Document document, LCS baseLCS)
{
    // Создание рабочей плоскости
    LCSWorkplane workplane = new LCSWorkplane(document);
    workplane.LCS = baseLCS;
    
    // Создание группы трансформаций
    TransformationGroup transformGroup = workplane.Transformations.AddBaseTransfGroup();
    transformGroup.SetLCS(baseLCS, true);
    
    // Добавление последовательных трансформаций
    transformGroup.AddMoveTransf(TransformationCoordinate.X, 50.0);
    transformGroup.AddRotateTransf(TransformationCoordinate.Z, Math.PI / 4);
    transformGroup.AddScaleTransf(TransformationCoordinate.X, 1.5);
    
    // Применение трансформации к объекту
    // (предполагается, что у нас есть modelObject)
    // modelObject.Transform(transformGroup);
}
```

### Работа с узлами и размерами в 3D

```csharp
public void CreateDimensionedModel(Document document, ShaftData shaftData)
{
    // Получение узлов модели
    Node3D node1 = Utils.GetNodeByStepIndex(document, 0);
    Node3D node2 = Utils.GetNodeByStepIndex(document, 1);
    
    // Создание координат размера
    DimensionUVCoords coords = new DimensionUVCoords();
    
    // Создание линейного размера
    LinearDimension3D dimension = new LinearDimension3D(document);
    
    // Настройка рабочей плоскости
    LCSWorkplane workplane = new LCSWorkplane(document);
    dimension.SetOrientationPlane(workplane);
    
    // Установка элементов размера
    dimension.SetElements(node1, Dimension3DElementType.Point, 
                         node2, Dimension3DElementType.Point, coords);
    
    // Установка отступов
    dimension.SetOffsets(20, 0, 0);
    
    // Расчет длины вала
    double shaftLength = 0;
    foreach (var step in shaftData.Parameters.shaftStepList)
    {
        shaftLength += step.GetLength();
    }
    
    // Установка ручного значения
    dimension.Value = shaftLength;
}
```

### Создание и манипуляция LCS с геометрией

```csharp
public LCS CreateCustomLCS(Document document, Point3D origin, Direction xDir, Direction yDir)
{
    // Создание PointsLCS
    PointsLCS lcs = new PointsLCS(document);
    lcs.Name = "CustomLCS";
    
    // Установка начала координат
    lcs.PointToOrigin = origin;
    
    // Установка направлений осей
    lcs.DirectionToAxisX = xDir;
    lcs.DirectionToAxisY = yDir;
    
    // Переключение осей для правильной ориентации
    lcs.SwitchAroundZ();
    lcs.SwitchAroundZ();
    lcs.SwitchAroundX();
    
    return lcs;
}
```

### Работа с аффинными преобразованиями

```csharp
public Point3D ApplyComplexTransformation(Point3D point, ModelAxis axis, double angle, Point3D translation)
{
    // Создание аффинного преобразования
    AffineTransformation transform = new AffineTransformation();
    
    // Вращение вокруг оси
    transform.Rotate(axis, angle);
    
    // Перенос
    transform.Translate(translation.X, translation.Y, translation.Z);
    
    // Масштабирование
    transform.Scale(1.2, 1.0, 1.0);
    
    // Применение преобразования к точке
    return point * transform;
}
```

### Создание проекции с трансформациями

```csharp
public Projection CreateTransformedProjection(Document document, ModelObject modelObject)
{
    // Создание простой проекции
    SimpleDrawingProjection projection = new SimpleDrawingProjection(document);
    projection.AddBody(modelObject as Operation);
    
    // Установка типа вида
    projection.SetViewType(ProjectionViewType.Front);
    
    // Получение LCS шага
    LCS stepLCS = Utils.GetLCSByStepIndex(document, 0, false);
    
    // Создание LCS для проекции
    PointsLCS projLCS = new PointsLCS(document);
    projLCS.Name = "ProjectionLCS";
    projLCS.PointToOrigin = stepLCS.Geometry.Origin;
    projLCS.DirectionToAxisX = stepLCS.Geometry.DirectionX;
    projLCS.DirectionToAxisY = stepLCS.Geometry.DirectionY;
    
    // Создание рабочей плоскости
    LCSWorkplane wp = new LCSWorkplane(document);
    wp.LCS = projLCS;
    
    // Добавление трансформаций
    TransformationGroup transfGroup = wp.Transformations.AddBaseTransfGroup();
    transfGroup.SetLCS(projLCS, true);
    transfGroup.AddRotateTransf(TransformationCoordinate.X, Math.PI / 6); // 30 градусов
    
    // Установка рабочей плоскости проекции
    projection.SetViewWorkplane(wp);
    
    // Установка масштаба
    projection.Scale = new Parameter(2.0);
    
    // Позиционирование на листе
    double posX = (document.ActivePage.Right.Value - document.ActivePage.Left.Value) / 2;
    double posY = (document.ActivePage.Top.Value - document.ActivePage.Bottom.Value) / 2;
    projection.SetTiePoint(posX, posY);
    
    return projection;
}
```

### Работа с параметрами модели

```csharp
public void ManipulateModelParameters(Document document)
{
    // Получение активной страницы
    var page = document.ActivePage;
    
    // Работа с параметрами страницы
    double width = page.Properties.Paper.Width;
    double height = page.Properties.Paper.Height;
    
    // Создание параметра с выражением
    Parameter dynamicScale = new Parameter();
    dynamicScale.Expression = "PageWidth / 100"; // Пример выражения
    
    // Использование в модели
    // projection.Scale = dynamicScale;
    
    // Получение линейных единиц
    var units = document.Properties.LinearUnit;
    double coeff = units.CoefficientToBase;
    
    // Преобразование координат
    Point3D worldPoint = new Point3D(100, 200, 0);
    Point3D modelPoint = new Point3D(
        worldPoint.X * coeff,
        worldPoint.Y * coeff,
        worldPoint.Z * coeff
    );
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D_Advanced_Examples.md
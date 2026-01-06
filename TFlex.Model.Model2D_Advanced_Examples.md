# Продвинутые примеры использования классов в пространстве имён TFlex.Model.Model2D

## Комплексные сценарии работы с 2D-объектами

### Создание полной 2D-проекции вала с размерами

```csharp
public Projection CreateDetailedShaftProjection(Document document, ModelObject modelObject, ShaftData shaftData)
{
    document.BeginChanges("Создание детальной проекции вала");
    
    // Удаление существующих объектов проекции
    DeleteAllProjectionObjects(document);
    
    // Создание проекции
    SimpleDrawingProjection projection = new SimpleDrawingProjection(document);
    projection.AddBody(modelObject as Operation);
    
    // Настройка вида
    projection.SetViewType(shaftData.Parameters.Draw.ProjectionViewType);
    
    // Получение LCS первого шага
    LCS stepLCS = Utils.GetLCSByStepIndex(document, 0, false);
    
    // Создание LCS для проекции
    PointsLCS projLCS = new PointsLCS(document) { Name = "ProjectionLCS" };
    projLCS.PointToOrigin = stepLCS.Geometry.Origin;
    projLCS.DirectionToAxisX = stepLCS.Geometry.DirectionX;
    projLCS.DirectionToAxisY = stepLCS.Geometry.DirectionY;
    projLCS.SwitchAroundZ();
    projLCS.SwitchAroundZ();
    projLCS.SwitchAroundX();
    
    // Создание рабочей плоскости
    LCSWorkplane wp = new LCSWorkplane(document);
    wp.LCS = projLCS;
    
    // Добавление вращения проекции
    TransformationGroup transfGroup = wp.Transformations.AddBaseTransfGroup();
    transfGroup.SetLCS(projLCS, true);
    transfGroup.AddRotateTransf(TransformationCoordinate.X, shaftData.Parameters.Draw.ProjectionRotateAng.Value);
    
    // Настройка проекции
    projection.Scale = new Parameter(2.0);
    
    double posX = (document.ActivePage.Right.Value - document.ActivePage.Left.Value) / 2;
    double posY = (document.ActivePage.Top.Value - document.ActivePage.Bottom.Value) / 2;
    projection.SetTiePoint(posX, posY);
    
    // Добавление размеров
    AddShaftDimensions(document, shaftData, projection.Scale.Value);
    
    document.EndChanges();
    return projection;
}
```

### Создание системы размеров для вала

```csharp
private void AddShaftDimensions(Document document, ShaftData shaftData, double scale)
{
    double posX = (document.ActivePage.Right.Value - document.ActivePage.Left.Value) / 2;
    double posY = (document.ActivePage.Top.Value - document.ActivePage.Bottom.Value) / 2;
    
    // Расчет общей длины вала
    double shaftLength = 0;
    double dMax = 0;
    foreach (var step in shaftData.Parameters.shaftStepList)
    {
        shaftLength += step.GetLength();
        double d = step.GetDiameterMax();
        if (d > dMax) dMax = d;
    }
    
    double x = shaftLength / 2;
    double y = 0;
    
    // Создание начального и конечного узлов
    FreeNode nodeBegin = new FreeNode(document);
    nodeBegin.X = x * scale + posX;
    nodeBegin.Y = y + posY;
    
    FreeNode nodeEnd = new FreeNode(document);
    nodeEnd.X = x * scale + posX;
    nodeEnd.Y = y + posY;
    
    double offset = (dMax / 2) * scale + 24;
    
    // Создание размеров для каждого шага
    for (int stepIndex = 0; stepIndex < shaftData.Parameters.shaftStepList.Count; stepIndex++)
    {
        double stepLength = shaftData.Parameters.shaftStepList[stepIndex].GetLength();
        
        FreeNode node1 = new FreeNode(document);
        node1.X = x * scale + posX;
        node1.Y = y + posY;
        
        x -= stepLength;
        
        FreeNode node2 = new FreeNode(document);
        node2.X = x * scale + posX;
        node2.Y = y + posY;
        
        nodeEnd.X = x * scale + posX;
        nodeEnd.Y = y + posY;
        
        // Размер для шага (кроме последнего)
        if (stepIndex < shaftData.Parameters.shaftStepList.Count - 1)
        {
            LinearDimension stepDimension = new LinearDimension(document);
            stepDimension.SetTwoNodes(node1, node2, DimensionAlignType.Horizontal);
            stepDimension.SetOffsets(null, offset, null, 0, null, 0);
            stepDimension.ValueType = DimensionValueType.Manual;
            stepDimension.Value = stepLength;
        }
    }
    
    // Общий размер длины
    offset += 24;
    LinearDimension totalDimension = new LinearDimension(document);
    totalDimension.SetTwoNodes(nodeBegin, nodeEnd, DimensionAlignType.Horizontal);
    totalDimension.SetOffsets(null, offset, null, 0, null, 0);
    totalDimension.ValueType = DimensionValueType.Manual;
    totalDimension.Value = shaftLength;
}
```

### Работа с различными типами выравнивания размеров

```csharp
public void DemonstrateDimensionAlignments(Document document)
{
    // Создание тестовых узлов
    FreeNode node1 = new FreeNode(document, 50, 50);
    FreeNode node2 = new FreeNode(document, 150, 50);
    FreeNode node3 = new FreeNode(document, 50, 150);
    FreeNode node4 = new FreeNode(document, 150, 150);
    
    // Горизонтальный размер
    LinearDimension horizDim = new LinearDimension(document);
    horizDim.SetTwoNodes(node1, node2, DimensionAlignType.Horizontal);
    horizDim.SetOffsets(null, -20, null, 0, null, 0);
    
    // Вертикальный размер
    LinearDimension vertDim = new LinearDimension(document);
    vertDim.SetTwoNodes(node1, node3, DimensionAlignType.Vertical);
    vertDim.SetOffsets(-20, null, null, 0, null, 0);
    
    // Параллельный размер (диагональный)
    LinearDimension parallelDim = new LinearDimension(document);
    parallelDim.SetTwoNodes(node1, node4, DimensionAlignType.Parallel);
    parallelDim.SetOffsets(null, null, 20, 0, 0, 0);
}
```

### Динамическое управление значениями размеров

```csharp
public void CreateDynamicDimensions(Document document)
{
    // Создание узлов
    FreeNode startNode = new FreeNode(document, 0, 0);
    FreeNode endNode = new FreeNode(document, 100, 0);
    
    // Размер с автоматическим значением
    LinearDimension autoDimension = new LinearDimension(document);
    autoDimension.SetTwoNodes(startNode, endNode, DimensionAlignType.Horizontal);
    autoDimension.ValueType = DimensionValueType.Auto;
    // Значение будет рассчитано автоматически
    
    // Размер с параметром
    Parameter lengthParam = new Parameter(100.0);
    LinearDimension paramDimension = new LinearDimension(document);
    paramDimension.SetTwoNodes(startNode, endNode, DimensionAlignType.Horizontal);
    paramDimension.ValueType = DimensionValueType.Parameter;
    paramDimension.Parameter = lengthParam;
    
    // Изменение параметра повлияет на размер
    lengthParam.Value = 150.0;
    
    // Ручной размер с выражением
    LinearDimension exprDimension = new LinearDimension(document);
    exprDimension.SetTwoNodes(startNode, endNode, DimensionAlignType.Horizontal);
    exprDimension.ValueType = DimensionValueType.Manual;
    exprDimension.Value = 200.0; // Фиксированное значение
}
```

### Удаление объектов проекции

```csharp
private void DeleteAllProjectionObjects(Document document)
{
    ObjectArray objectsToDelete = new ObjectArray();
    
    // Получение всех объектов документа
    ICollection<ModelObject> objList = document.GetObjects();
    foreach (ModelObject obj in objList)
    {
        // Удаление объектов типа Projection
        if (obj.GroupType == ObjectType.Projection)
        {
            objectsToDelete.Add(obj);
        }
    }
    
    // Удаление LCS проекции
    ModelObject projLCS = document.GetObjectByName("ProjectionLCS");
    if (projLCS != null)
    {
        objectsToDelete.Add(projLCS);
    }
    
    // Выполнение удаления с опциями
    DeleteOptions deleteOptions = new DeleteOptions(true);
    document.DeleteObjects(objectsToDelete, deleteOptions);
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model2D_Advanced_Examples.md
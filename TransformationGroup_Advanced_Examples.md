# Продвинутые примеры использования класса TransformationGroup в T-Flex CAD API

## Продвинутые сценарии использования трансформаций

### 1. Комбинированные трансформации с параметрическим управлением

```csharp
public class AdvancedTransformationExample
{
    public void CreateParametricTransformations(Object3D targetObject)
    {
        // Получаем контейнер трансформаций
        TransformationGroupContainer container = targetObject.Transformations;
        
        // Создаем группу для параметрических трансформаций
        TransformationGroup paramGroup = container.AddBaseTransfGroup();
        paramGroup.Name = "Параметрические трансформации";
        
        // Создаем параметры для управления трансформациями
        Parameter xOffset = new Parameter("Смещение по X", 25.0, "мм");
        Parameter yOffset = new Parameter("Смещение по Y", 15.0, "мм");
        Parameter rotationAngle = new Parameter("Угол поворота", 30.0, "град");
        
        // Добавляем параметризованные перемещения
        paramGroup.AddMoveTransf(TransformationCoordinate.X, xOffset);
        paramGroup.AddMoveTransf(TransformationCoordinate.Y, yOffset);
        
        // Добавляем параметризованное вращение
        paramGroup.AddRotateTransf(TransformationCoordinate.Z, rotationAngle);
        
        // Можно также связать параметры с внешними источниками данных
        // Например, с таблицей параметров или пользовательским интерфейсом
    }
}
```

### 2. Создание трансформаций на основе геометрических объектов

```csharp
public class GeometryBasedTransformation
{
    public void AlignObjectToSurface(Object3D objectToAlign, ModelSurface targetSurface)
    {
        TransformationGroupContainer container = objectToAlign.Transformations;
        TransformationGroup alignmentGroup = container.AddBaseTransfGroup();
        alignmentGroup.Name = "Выравнивание по поверхности";
        
        // Перемещаем объект до плоскости
        alignmentGroup.AddMoveToSurfaceTransf(TransformationCoordinate.Z, targetSurface);
        
        // Дополнительно можно добавить выравнивание нормали поверхности
        // (предполагается, что у ModelSurface есть метод получения нормали)
        ModelDirection surfaceNormal = targetSurface.GetNormal();
        alignmentGroup.AddSetAxisDirectionTransf(TransformationCoordinate.Z, surfaceNormal);
    }
    
    public void AlignToObjectAxis(Object3D objectToAlign, ModelAxis targetAxis)
    {
        TransformationGroupContainer container = objectToAlign.Transformations;
        TransformationGroup alignmentGroup = container.AddBaseTransfGroup();
        alignmentGroup.Name = "Выравнивание по оси";
        
        // Совмещаем ось объекта с целевой осью
        alignmentGroup.AddSetAxisTransf(TransformationCoordinate.X, targetAxis);
    }
}
```

### 3. Создание трансформаций для движения по кривой

```csharp
public class CurveFollowingTransformation
{
    public void FollowCurvePath(Object3D movingObject, ModelCurve pathCurve, Parameter positionParameter)
    {
        TransformationGroupContainer container = movingObject.Transformations;
        TransformationGroup motionGroup = container.AddBaseTransfGroup();
        motionGroup.Name = "Движение по кривой";
        
        // Перемещаем объект вдоль кривой
        motionGroup.AddMoveToCurveTransf(TransformationCoordinate.X, pathCurve);
        
        // Можно добавить ориентацию объекта по касательной к кривой
        // Это требует дополнительных вычислений для получения направления касательной
        ModelDirection tangentDirection = pathCurve.GetTangentAtParameter(positionParameter.Value);
        motionGroup.AddSetAxisDirectionTransf(TransformationCoordinate.X, tangentDirection);
    }
}
```

### 4. Создание сложных трансформаций с использованием матриц

```csharp
public class MatrixTransformationExample
{
    public void ApplyComplexTransformation(Object3D targetObject)
    {
        TransformationGroupContainer container = targetObject.Transformations;
        TransformationGroup matrixGroup = container.AddBaseTransfGroup();
        matrixGroup.Name = "Матричная трансформация";
        
        // Создаем сложную аффинную трансформацию
        AffineTransformation complexTransform = new AffineTransformation();
        
        // Комбинируем масштабирование, поворот и перемещение
        complexTransform.Scale(1.5, 1.2, 1.0); // Масштабирование
        complexTransform.RotateZ(45.0);        // Поворот вокруг Z
        complexTransform.Translate(20.0, 10.0, 0.0); // Перемещение
        
        // Применяем матрицу трансформации
        matrixGroup.AddMap(complexTransform);
    }
}
```

### 5. Создание трансформаций для системы координат

```csharp
public class CoordinateSystemTransformation
{
    public void SetCustomCoordinateSystem(Object3D targetObject, ModelPoint3D origin, 
                                        ModelDirection xAxis, ModelDirection yAxis)
    {
        TransformationGroupContainer container = targetObject.Transformations;
        TransformationGroup csGroup = container.AddBaseTransfGroup();
        csGroup.Name = "Пользовательская СК";
        
        // Создаем новую ЛСК
        LCS customLCS = new LCS();
        customLCS.SetOrigin(origin);
        customLCS.SetXAxis(xAxis);
        customLCS.SetYAxis(yAxis);
        
        // Устанавливаем пользовательскую ЛСК для группы
        csGroup.SetLCS(customLCS, true);
    }
}
```

### 6. Управление порядком трансформаций

```csharp
public class TransformationOrderManagement
{
    public void ReorderTransformations(Object3D targetObject)
    {
        TransformationGroupContainer container = targetObject.Transformations;
        
        // Создаем несколько групп трансформаций в определенном порядке
        TransformationGroup rotationGroup = container.AddBaseTransfGroup();
        rotationGroup.Name = "Поворот";
        rotationGroup.AddRotateTransf(TransformationCoordinate.Z, new Parameter(45.0));
        
        TransformationGroup translationGroup = container.AddBaseTransfGroup();
        translationGroup.Name = "Перемещение";
        translationGroup.AddMoveTransf(TransformationCoordinate.X, new Parameter(50.0));
        
        // Если нужно изменить порядок, перемещаем группы
        // Перемещаем группу поворота после группы перемещения
        container.MoveBaseTransfGroupDown(rotationGroup);
    }
}
```

### 7. Условные трансформации

```csharp
public class ConditionalTransformation
{
    public void ApplyConditionalTransform(Object3D targetObject, bool condition)
    {
        TransformationGroupContainer container = targetObject.Transformations;
        TransformationGroup conditionalGroup = container.AddBaseTransfGroup();
        conditionalGroup.Name = "Условная трансформация";
        
        if (condition)
        {
            // Применяем одно преобразование
            conditionalGroup.AddMoveTransf(TransformationCoordinate.X, new Parameter(100.0));
        }
        else
        {
            // Применяем другое преобразование
            conditionalGroup.AddRotateTransf(TransformationCoordinate.Z, new Parameter(90.0));
        }
        
        // Можно также использовать параметр для управления подавлением
        Parameter suppressionParam = new Parameter(condition ? 0.0 : 1.0);
        conditionalGroup.Suppressed = suppressionParam;
    }
}
```

### 8. Создание трансформаций для зеркального отображения

```csharp
public class MirrorTransformation
{
    public void CreateMirrorTransform(Object3D targetObject, ModelSurface mirrorPlane)
    {
        TransformationGroupContainer container = targetObject.Transformations;
        TransformationGroup mirrorGroup = container.AddBaseTransfGroup();
        mirrorGroup.Name = "Зеркальное отображение";
        
        // Для создания зеркального отображения можно использовать
        // комбинацию поворотов и масштабирования
        AffineTransformation mirrorTransform = new AffineTransformation();
        
        // Отражение относительно плоскости YZ (изменение знака X)
        mirrorTransform.Scale(-1.0, 1.0, 1.0);
        
        // Перемещаем объект так, чтобы плоскость отражения совпадала с YZ
        ModelPoint3D planePoint = mirrorPlane.GetPoint();
        mirrorTransform.Translate(-2 * planePoint.X, 0.0, 0.0);
        
        mirrorGroup.AddMap(mirrorTransform);
    }
}
```

### 9. Анимация трансформаций

```csharp
public class AnimatedTransformation
{
    public void CreateAnimationTransform(Object3D targetObject, Parameter animationParameter)
    {
        TransformationGroupContainer container = targetObject.Transformations;
        TransformationGroup animationGroup = container.AddBaseTransfGroup();
        animationGroup.Name = "Анимационная трансформация";
        
        // Создаем параметризованные трансформации для анимации
        // Например, плавное перемещение в зависимости от параметра анимации
        Parameter animatedOffset = new Parameter();
        animatedOffset.SetExpression("Анимация * 100"); // Зависимость от параметра
        
        animationGroup.AddMoveTransf(TransformationCoordinate.X, animatedOffset);
        
        // Можно также анимировать поворот
        Parameter animatedRotation = new Parameter();
        animatedRotation.SetExpression("Анимация * 360"); // Полный оборот
        
        animationGroup.AddRotateTransf(TransformationCoordinate.Z, animatedRotation);
    }
}
```

### 10. Работа с множественными трансформациями

```csharp
public class MultipleTransformations
{
    public void CreateComplexTransform(Object3D targetObject)
    {
        TransformationGroupContainer container = targetObject.Transformations;
        
        // Создаем несколько групп для разных типов трансформаций
        TransformationGroup baseGroup = container.AddBaseTransfGroup();
        baseGroup.Name = "Базовая трансформация";
        baseGroup.AddMoveTransf(TransformationCoordinate.X, new Parameter(50.0));
        
        TransformationGroup detailGroup = container.AddBaseTransfGroup();
        detailGroup.Name = "Детализация";
        detailGroup.AddRotateTransf(TransformationCoordinate.Z, new Parameter(15.0));
        
        TransformationGroup fineTuneGroup = container.AddBaseTransfGroup();
        fineTuneGroup.Name = "Точная настройка";
        fineTuneGroup.AddMoveTransf(TransformationCoordinate.Y, new Parameter(5.0));
        
        // Можно управлять подавлением отдельных групп
        Parameter suppression = new Parameter(0.0); // 0 - активна, >0 - подавлена
        detailGroup.Suppressed = suppression;
    }
}
```

Эти продвинутые примеры демонстрируют сложные сценарии использования трансформаций в T-Flex CAD API, включая параметрическое управление, работу с геометрическими объектами, матричные трансформации и создание сложных анимационных эффектов.
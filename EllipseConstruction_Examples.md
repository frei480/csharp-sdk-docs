# Примеры использования класса EllipseConstruction в T-Flex CAD API

## Описание класса

Класс `EllipseConstruction` представляет собой линию построения в виде эллипса в 2D-пространстве. Он наследуется от класса `Construction` и предоставляет функциональность для создания различных типов эллипсов построения.

## Конструкторы

### 1. EllipseConstruction(Document)

Конструктор по умолчанию для создания эллипса построения.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание эллипса построения");

// Создание эллипса построения
EllipseConstruction ellipse = new EllipseConstruction(document);

// Закрытие блока изменений документа
document.EndChanges();
```

## Основные методы создания эллипсов

### 1. Создание эллипса с центром и двумя узлами
```csharp
public static void CreateEllipseWithCenterAndTwoNodes()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание эллипса с центром и двумя узлами");
    
    // Создание узлов
    int r1 = 50;
    int r2 = 30;
    
    FreeNode fnCenter = new FreeNode(document, 50, 100);
    FreeNode fn1 = new FreeNode(document, fnCenter.X.Value + r1, fnCenter.Y.Value);
    FreeNode fn2 = new FreeNode(document, fnCenter.X.Value, fnCenter.Y.Value + r2);
    
    // Создание эллипса построения
    EllipseConstruction ec = new EllipseConstruction(document);
    ec.SetCenterAndTwoNodes(fnCenter, fn1, fn2);
    
    document.EndChanges();
}
```

### 2. Создание эллипса через три узла
```csharp
public static void CreateEllipseThroughThreeNodes()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание эллипса через три узла");
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 10, 50);
    FreeNode fn2 = new FreeNode(document, 90, 50);
    FreeNode fn3 = new FreeNode(document, 50, 80);
    
    // Создание эллипса построения
    EllipseConstruction ellipse = new EllipseConstruction(document);
    ellipse.SetThreeNodes(fn1, fn2, fn3);
    
    document.EndChanges();
}
```

### 3. Создание эллипса с центром, узлом и радиусом
```csharp
public static void CreateEllipseWithCenterNodeAndRadius()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание эллипса с центром, узлом и радиусом");
    
    // Создание узлов
    FreeNode center = new FreeNode(document, 50, 50);
    FreeNode node = new FreeNode(document, 80, 50);
    
    // Создание эллипса построения
    EllipseConstruction ellipse = new EllipseConstruction(document);
    ellipse.SetCenterAndNodeAndRadius(center, node, 20);
    
    document.EndChanges();
}
```

## Свойства класса

### Основные свойства:

1. **SubType** - Подтип линии построения (всегда EllipseConstruction)
2. **GeometryType** - Тип геометрии линии построения (эллипс)
3. **ConstructionGeometry** - Геометрия линии построения
4. **EllipseConstructionGeometry** - Геометрия линии построения (эллипса)
5. **EllipseType** - Тип привязки эллипса

### Пример работы со свойствами:
```csharp
public static void WorkWithEllipseProperties()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Работа со свойствами эллипса");
    
    // Создание узлов
    FreeNode fnCenter = new FreeNode(document, 50, 100);
    FreeNode fn1 = new FreeNode(document, 100, 100);
    FreeNode fn2 = new FreeNode(document, 50, 130);
    
    // Создание эллипса построения
    EllipseConstruction ellipse = new EllipseConstruction(document);
    ellipse.SetCenterAndTwoNodes(fnCenter, fn1, fn2);
    
    // Получение свойств
    ConstructionType subType = ellipse.SubType;  // EllipseConstruction
    ObjectGeometryType geomType = ellipse.GeometryType; // Ellipse
    
    // Установка свойств отображения
    ellipse.Color = 255;    // Красный цвет
    ellipse.Layer = 2;      // Слой 2
    ellipse.Visible = true; // Видимость
    
    document.EndChanges();
}
```

## Примеры использования в контексте других объектов

### Создание эллипса касательного к прямой:
```csharp
public static void CreateEllipseTangentToLine()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание эллипса касательного к прямой");
    
    // Создание прямой
    FreeNode lineNode1 = new FreeNode(document, 10, 10);
    FreeNode lineNode2 = new FreeNode(document, 90, 10);
    LineConstruction line = new LineConstruction(document);
    line.SetThroughNodes(lineNode1, lineNode2);
    
    // Создание узлов
    FreeNode center = new FreeNode(document, 50, 50);
    FreeNode node = new FreeNode(document, 70, 50);
    
    // Создание эллипса построения
    EllipseConstruction ellipse = new EllipseConstruction(document);
    ellipse.SetCenterAndLineAndNode(center, line, node);
    
    document.EndChanges();
}
```

### Создание эллипса касательного к окружности:
```csharp
public static void CreateEllipseTangentToCircle()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание эллипса касательного к окружности");
    
    // Создание окружности
    FreeNode circleCenter = new FreeNode(document, 50, 50);
    CircleConstruction circle = new CircleConstruction(document);
    circle.SetCenterAndRadius(circleCenter, 20);
    
    // Создание узла
    FreeNode node = new FreeNode(document, 80, 80);
    
    // Создание эллипса построения
    EllipseConstruction ellipse = new EllipseConstruction(document);
    ellipse.SetCircleAndNode(circle, node);
    
    document.EndChanges();
}
```

## Типы линий построения в T-Flex CAD API

Класс `EllipseConstruction` является одним из основных типов линий построения в T-Flex CAD API:

1. **LineConstruction** - Прямые линии
2. **CircleConstruction** - Окружности
3. **EllipseConstruction** - Эллипсы
4. **PathConstruction** - Пути
5. **CopyConstruction** - Копии
6. **OffsetConstruction** - Эквидистанты
7. **SplineConstruction** - Сплайны
8. **FunctionConstruction** - Функции
9. **SymmetryConstruction** - Симметричные линии

## Наследование

Класс `EllipseConstruction` наследуется от следующей цепочки классов:
```
System.Object 
  TFlex.Model.ModelObject 
    TFlex.Model.Model2D.Object2D 
      TFlex.Model.Model2D.Construction 
        TFlex.Model.Model2D.EllipseConstruction
```

Это означает, что он наследует все свойства и методы этих классов, включая:
- Свойства отображения (цвет, слой, уровень)
- Свойства геометрии
- Свойства видимости и идентификации
- Методы работы с документом

## Практические рекомендации

1. **Всегда используйте блоки изменений документа** при создании или модификации объектов:
   ```csharp
   document.BeginChanges("Описание изменений");
   // Создание/модификация объектов
   document.EndChanges();
   ```

2. **Проверяйте существование документа** перед созданием объектов:
   ```csharp
   if (TFlex.Application.ActiveDocument != null)
   {
       Document document = TFlex.Application.ActiveDocument;
       // Работа с документом
   }
   ```

3. **Используйте соответствующие методы** для создания нужного типа эллипса:
   - `SetCenterAndTwoNodes()` для эллипса с центром и двумя узлами
   - `SetThreeNodes()` для эллипса через три узла
   - `SetCenterAndNodeAndRadius()` для эллипса с центром, узлом и радиусом

4. **Управляйте свойствами отображения** для лучшей визуализации:
   ```csharp
   ellipse.Color = 255;  // Красный цвет
   ellipse.Layer = 2;   // Слой 2
   ```

Эти примеры охватывают основные аспекты работы с классом `EllipseConstruction` в T-Flex CAD API и могут быть использованы в базе знаний для RAG-системы.
# Примеры использования класса PathConstruction в T-Flex CAD API

## Описание класса

Класс `PathConstruction` представляет собой линию построения в виде пути в 2D-пространстве. Он наследуется от класса `Construction` и предоставляет функциональность для создания путей построения, состоящих из различных сегментов.

## Конструкторы

### 1. PathConstruction(Document)

Конструктор по умолчанию для создания пути построения.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание пути построения");

// Создание пути построения
PathConstruction path = new PathConstruction(document);

// Закрытие блока изменений документа
document.EndChanges();
```

## Основные свойства класса

### 1. Contour - Контур пути
### 2. Length - Длина пути
### 3. PolylineConstructionGeometry - Геометрия линии построения (полилиния)

## Основные методы создания путей

### 1. Создание пути с контуром из линий изображения
```csharp
public static void CreatePathWithOutlineContour()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание пути с контуром");
    
    // Создание пути построения
    PathConstruction pathConstruction = new PathConstruction(document);
    Contour cn = pathConstruction.Contour; // Получение контура
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, -200, 50);
    FreeNode fn2 = new FreeNode(document, -160, 100);
    FreeNode fn3 = new FreeNode(document, -120, 50);
    FreeNode fn4 = new FreeNode(document, -80, 100);
    
    // Создание линий изображения
    ConstructionOutline l1 = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline l2 = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline l3 = new ConstructionOutline(document, fn3, fn4);
    
    // Создание дуги окружности
    double r = 68;
    TwoPointArcOutline twoPointArcOutline = new TwoPointArcOutline(document, fn4, fn1, r);
    
    // Создание сегментов контура
    OutlineContourSegment s1 = new OutlineContourSegment(cn);
    OutlineContourSegment s2 = new OutlineContourSegment(cn);
    OutlineContourSegment s3 = new OutlineContourSegment(cn);
    OutlineContourSegment s4 = new OutlineContourSegment(cn);
    
    // Назначение линий сегментам
    s1.Outline = l1;
    s2.Outline = l2;
    s3.Outline = l3;
    s4.Outline = twoPointArcOutline;
    
    document.EndChanges();
}
```

### 2. Создание простого пути из линий
```csharp
public static void CreateSimplePath()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание простого пути");
    
    // Создание пути построения
    PathConstruction path = new PathConstruction(document);
    Contour contour = path.Contour;
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 0, 0);
    FreeNode fn2 = new FreeNode(document, 50, 0);
    FreeNode fn3 = new FreeNode(document, 50, 50);
    FreeNode fn4 = new FreeNode(document, 0, 50);
    
    // Создание линий изображения
    ConstructionOutline line1 = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline line2 = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline line3 = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline line4 = new ConstructionOutline(document, fn4, fn1);
    
    // Создание сегментов контура
    OutlineContourSegment segment1 = new OutlineContourSegment(contour);
    OutlineContourSegment segment2 = new OutlineContourSegment(contour);
    OutlineContourSegment segment3 = new OutlineContourSegment(contour);
    OutlineContourSegment segment4 = new OutlineContourSegment(contour);
    
    // Назначение линий сегментам
    segment1.Outline = line1;
    segment2.Outline = line2;
    segment3.Outline = line3;
    segment4.Outline = line4;
    
    document.EndChanges();
}
```

### 3. Создание пути с дугами
```csharp
public static void CreatePathWithArcs()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание пути с дугами");
    
    // Создание пути построения
    PathConstruction path = new PathConstruction(document);
    Contour contour = path.Contour;
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 0, 0);
    FreeNode fn2 = new FreeNode(document, 100, 0);
    FreeNode fn3 = new FreeNode(document, 100, 100);
    FreeNode fn4 = new FreeNode(document, 0, 100);
    
    // Создание линий и дуг
    ConstructionOutline line1 = new ConstructionOutline(document, fn1, fn2);
    
    // Создание дуги через центр
    FreeNode center = new FreeNode(document, 100, 50);
    CircleConstruction circle = new CircleConstruction(document);
    circle.SetCenterAndRadius(center, 50);
    ConstructionOutline arc = new ConstructionOutline(document, fn2, fn3, circle);
    
    ConstructionOutline line2 = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline line3 = new ConstructionOutline(document, fn4, fn1);
    
    // Создание сегментов контура
    OutlineContourSegment s1 = new OutlineContourSegment(contour);
    OutlineContourSegment s2 = new OutlineContourSegment(contour);
    OutlineContourSegment s3 = new OutlineContourSegment(contour);
    OutlineContourSegment s4 = new OutlineContourSegment(contour);
    
    // Назначение линий сегментам
    s1.Outline = line1;
    s2.Outline = arc;
    s3.Outline = line2;
    s4.Outline = line3;
    
    document.EndChanges();
}
```

## Свойства класса

### Основные свойства:

1. **SubType** - Подтип линии построения (всегда PathConstruction)
2. **GeometryType** - Тип геометрии линии построения (путь)
3. **ConstructionGeometry** - Геометрия линии построения
4. **Contour** - Контур пути
5. **Length** - Длина пути
6. **PolylineConstructionGeometry** - Геометрия линии построения (полилиния)

### Пример работы со свойствами:
```csharp
public static void WorkWithPathProperties()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Работа со свойствами пути");
    
    // Создание пути построения
    PathConstruction path = new PathConstruction(document);
    
    // Получение свойств
    ConstructionType subType = path.SubType;  // PathConstruction
    ObjectGeometryType geomType = path.GeometryType; // Path
    double length = path.Length; // Длина пути
    
    // Получение контура
    Contour contour = path.Contour;
    
    // Установка свойств отображения
    path.Color = 255;    // Красный цвет
    path.Layer = 2;      // Слой 2
    path.Visible = true;  // Видимость
    
    document.EndChanges();
}
```

## Методы работы с путем

### 1. Получение угла наклона касательной
```csharp
public static void GetPathTangentAngle()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Получение угла касательной пути");
    
    // Создание пути построения
    PathConstruction path = new PathConstruction(document);
    Contour contour = path.Contour;
    
    // Создание узлов и линий (пример)
    FreeNode fn1 = new FreeNode(document, 0, 0);
    FreeNode fn2 = new FreeNode(document, 100, 100);
    ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);
    
    OutlineContourSegment segment = new OutlineContourSegment(contour);
    segment.Outline = line;
    
    // Получение угла наклона касательной в заданной точке пути
    double angle = path.GetAngle(0.5); // Угол в середине пути
    
    document.EndChanges();
}
```

### 2. Получение точки на пути
```csharp
public static void GetPointOnPath()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Получение точки на пути");
    
    // Создание пути построения
    PathConstruction path = new PathConstruction(document);
    Contour contour = path.Contour;
    
    // Создание узлов и линий (пример)
    FreeNode fn1 = new FreeNode(document, 0, 0);
    FreeNode fn2 = new FreeNode(document, 100, 0);
    ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);
    
    OutlineContourSegment segment = new OutlineContourSegment(contour);
    segment.Outline = line;
    
    // Получение точки на пути
    Point2D point = path.GetRelativePointToBegin(0.75); // Точка на 75% пути
    
    document.EndChanges();
}
```

## Примеры использования в контексте других объектов

### Создание пути как эквидистанты к другой линии:
```csharp
public static void CreatePathAsOffset()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание пути как эквидистанты");
    
    // Создание базовой линии
    FreeNode lineNode1 = new FreeNode(document, 10, 10);
    FreeNode lineNode2 = new FreeNode(document, 50, 10);
    LineConstruction baseLine = new LineConstruction(document);
    baseLine.SetThroughNodes(lineNode1, lineNode2);
    
    // Создание пути построения
    PathConstruction path = new PathConstruction(document);
    Contour contour = path.Contour;
    
    // Создание узлов для пути
    FreeNode fn1 = new FreeNode(document, 10, 20);
    FreeNode fn2 = new FreeNode(document, 50, 20);
    
    // Создание линий изображения
    ConstructionOutline line1 = new ConstructionOutline(document, fn1, fn2);
    
    // Создание сегментов контура
    OutlineContourSegment segment = new OutlineContourSegment(contour);
    segment.Outline = line1;
    
    document.EndChanges();
}
```

### Создание замкнутого пути:
```csharp
public static void CreateClosedPath()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание замкнутого пути");
    
    // Создание пути построения
    PathConstruction path = new PathConstruction(document);
    Contour contour = path.Contour;
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 0, 0);
    FreeNode fn2 = new FreeNode(document, 100, 0);
    FreeNode fn3 = new FreeNode(document, 100, 100);
    FreeNode fn4 = new FreeNode(document, 0, 100);
    
    // Создание линий изображения
    ConstructionOutline line1 = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline line2 = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline line3 = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline line4 = new ConstructionOutline(document, fn4, fn1);
    
    // Создание сегментов контура
    OutlineContourSegment s1 = new OutlineContourSegment(contour);
    OutlineContourSegment s2 = new OutlineContourSegment(contour);
    OutlineContourSegment s3 = new OutlineContourSegment(contour);
    OutlineContourSegment s4 = new OutlineContourSegment(contour);
    
    // Назначение линий сегментам
    s1.Outline = line1;
    s2.Outline = line2;
    s3.Outline = line3;
    s4.Outline = line4;
    
    document.EndChanges();
}
```

## Типы линий построения в T-Flex CAD API

Класс `PathConstruction` является одним из основных типов линий построения в T-Flex CAD API:

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

Класс `PathConstruction` наследуется от следующей цепочки классов:
```
System.Object 
  TFlex.Model.ModelObject 
    TFlex.Model.Model2D.Object2D 
      TFlex.Model.Model2D.Construction 
        TFlex.Model.Model2D.PathConstruction
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

3. **Используйте соответствующие методы** для создания нужного типа пути:
   - Получайте контур через свойство `Contour`
   - Создавайте сегменты контура с помощью `OutlineContourSegment`
   - Назначайте линии изображения сегментам через свойство `Outline`

4. **Управляйте свойствами отображения** для лучшей визуализации:
   ```csharp
   path.Color = 255;  // Красный цвет
   path.Layer = 2;   // Слой 2
   ```

Эти примеры охватывают основные аспекты работы с классом `PathConstruction` в T-Flex CAD API и могут быть использованы в базе знаний для RAG-системы.
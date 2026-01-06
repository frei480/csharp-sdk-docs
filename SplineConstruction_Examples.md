# Примеры использования класса SplineConstruction в T-Flex CAD API

## Описание класса

Класс `SplineConstruction` представляет собой линию построения в виде сплайна в 2D-пространстве. Он наследуется от класса `Construction` и предоставляет функциональность для создания различных типов сплайнов построения.

## Конструкторы

### 1. SplineConstruction(Document)

Конструктор по умолчанию для создания сплайна построения.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание сплайна построения");

// Создание сплайна построения
SplineConstruction spline = new SplineConstruction(document);

// Закрытие блока изменений документа
document.EndChanges();
```

## Основные методы создания сплайнов

### 1. Создание сплайна с заданными точками
```csharp
public static void CreateSplineWithPoints()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание сплайна с точками");
    
    // Создание сплайна построения
    SplineConstruction sc = new SplineConstruction(document);
    sc.Color = 200;
    sc.Interpolating = false;
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 10, 200);
    FreeNode fn2 = new FreeNode(document, 30, 240);
    FreeNode fn3 = new FreeNode(document, 100, 240);
    
    // Добавление точек
    sc.StartTangentNode = fn1;
    sc.AddPoint(fn2);
    sc.AddPoint(fn3);
    
    document.EndChanges();
}
```

### 2. Создание замкнутого сплайна
```csharp
public static void CreateClosedSpline()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание замкнутого сплайна");
    
    // Создание сплайна построения
    SplineConstruction spline = new SplineConstruction(document);
    spline.Closed = true; // Замкнутый сплайн
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 10, 10);
    FreeNode fn2 = new FreeNode(document, 50, 10);
    FreeNode fn3 = new FreeNode(document, 50, 50);
    FreeNode fn4 = new FreeNode(document, 10, 50);
    
    // Добавление точек
    spline.StartTangentNode = fn1;
    spline.AddPoint(fn2);
    spline.AddPoint(fn3);
    spline.AddPoint(fn4);
    
    document.EndChanges();
}
```

### 3. Создание интерполяционного сплайна
```csharp
public static void CreateInterpolatingSpline()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание интерполяционного сплайна");
    
    // Создание сплайна построения
    SplineConstruction spline = new SplineConstruction(document);
    spline.Interpolating = true; // Интерполяционный сплайн
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 0, 0);
    FreeNode fn2 = new FreeNode(document, 30, 40);
    FreeNode fn3 = new FreeNode(document, 60, 20);
    FreeNode fn4 = new FreeNode(document, 90, 60);
    
    // Добавление точек
    spline.StartTangentNode = fn1;
    spline.AddPoint(fn2);
    spline.AddPoint(fn3);
    spline.AddPoint(fn4);
    
    document.EndChanges();
}
```

## Свойства класса

### Основные свойства:

1. **SubType** - Подтип линии построения (всегда SplineConstruction)
2. **GeometryType** - Тип геометрии линии построения (сплайн)
3. **ConstructionGeometry** - Геометрия линии построения
4. **Closed** - Замкнутый сплайн
5. **Interpolating** - Интерполяционный сплайн
6. **PointCount** - Количество точек сплайна
7. **StartTangentNode** - Узел, задающий касание в начале
8. **EndTangentNode** - Узел, задающий касание в конце

### Пример работы со свойствами:
```csharp
public static void WorkWithSplineProperties()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Работа со свойствами сплайна");
    
    // Создание сплайна построения
    SplineConstruction spline = new SplineConstruction(document);
    
    // Получение свойств
    ConstructionType subType = spline.SubType;  // SplineConstruction
    ObjectGeometryType geomType = spline.GeometryType; // Spline
    
    // Установка свойств сплайна
    spline.Closed = false;      // Незамкнутый сплайн
    spline.Interpolating = true; // Интерполяционный сплайн
    spline.Color = 255;         // Красный цвет
    spline.Layer = 2;           // Слой 2
    spline.Visible = true;      // Видимость
    
    document.EndChanges();
}
```

## Методы работы с точками сплайна

### 1. Добавление точек к сплайну
```csharp
public static void AddPointsToSpline()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Добавление точек к сплайну");
    
    SplineConstruction spline = new SplineConstruction(document);
    
    // Создание узлов
    FreeNode startNode = new FreeNode(document, 0, 0);
    FreeNode point1 = new FreeNode(document, 20, 30);
    FreeNode point2 = new FreeNode(document, 40, 10);
    FreeNode point3 = new FreeNode(document, 60, 40);
    
    // Установка начальной точки
    spline.StartTangentNode = startNode;
    
    // Добавление точек
    spline.AddPoint(point1);
    spline.AddPoint(point2);
    spline.AddPoint(point3);
    
    document.EndChanges();
}
```

### 2. Вставка точки в сплайн
```csharp
public static void InsertPointToSpline()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Вставка точки в сплайн");
    
    SplineConstruction spline = new SplineConstruction(document);
    
    // Создание узлов
    FreeNode startNode = new FreeNode(document, 0, 0);
    FreeNode point1 = new FreeNode(document, 30, 30);
    FreeNode point2 = new FreeNode(document, 60, 0);
    
    // Установка начальной точки
    spline.StartTangentNode = startNode;
    spline.AddPoint(point1);
    spline.AddPoint(point2);
    
    // Вставка новой точки
    FreeNode newPoint = new FreeNode(document, 15, 15);
    spline.InsertPoint(1, newPoint); // Вставка в позицию 1
    
    document.EndChanges();
}
```

### 3. Удаление точки из сплайна
```csharp
public static void DeletePointFromSpline()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Удаление точки из сплайна");
    
    SplineConstruction spline = new SplineConstruction(document);
    
    // Создание узлов
    FreeNode startNode = new FreeNode(document, 0, 0);
    FreeNode point1 = new FreeNode(document, 20, 30);
    FreeNode point2 = new FreeNode(document, 40, 10);
    FreeNode point3 = new FreeNode(document, 60, 40);
    
    // Установка начальной точки
    spline.StartTangentNode = startNode;
    spline.AddPoint(point1);
    spline.AddPoint(point2);
    spline.AddPoint(point3);
    
    // Удаление точки
    spline.DeletePoint(1); // Удаление точки в позиции 1
    
    document.EndChanges();
}
```

## Примеры использования в контексте других объектов

### Создание сплайна как эквидистанты к другой линии:
```csharp
public static void CreateSplineAsOffset()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание сплайна как эквидистанты");
    
    // Создание базовой линии
    FreeNode lineNode1 = new FreeNode(document, 10, 10);
    FreeNode lineNode2 = new FreeNode(document, 50, 10);
    LineConstruction baseLine = new LineConstruction(document);
    baseLine.SetThroughNodes(lineNode1, lineNode2);
    
    // Создание сплайна построения
    SplineConstruction spline = new SplineConstruction(document);
    spline.Interpolating = true;
    
    // Создание узлов для сплайна
    FreeNode fn1 = new FreeNode(document, 10, 20);
    FreeNode fn2 = new FreeNode(document, 30, 30);
    FreeNode fn3 = new FreeNode(document, 50, 20);
    
    // Добавление точек
    spline.StartTangentNode = fn1;
    spline.AddPoint(fn2);
    spline.AddPoint(fn3);
    
    document.EndChanges();
}
```

### Создание сплайна с заданными весами точек:
```csharp
public static void CreateSplineWithPointWeights()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание сплайна с весами точек");
    
    SplineConstruction spline = new SplineConstruction(document);
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 0, 0);
    FreeNode fn2 = new FreeNode(document, 30, 40);
    FreeNode fn3 = new FreeNode(document, 60, 20);
    
    // Добавление точек
    spline.StartTangentNode = fn1;
    spline.AddPoint(fn2);
    spline.AddPoint(fn3);
    
    // Установка весов точек
    spline.SetPointWeight(0, 1.0); // Вес начальной точки
    spline.SetPointWeight(1, 2.0); // Вес первой точки
    spline.SetPointWeight(2, 1.5); // Вес второй точки
    
    document.EndChanges();
}
```

## Типы линий построения в T-Flex CAD API

Класс `SplineConstruction` является одним из основных типов линий построения в T-Flex CAD API:

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

Класс `SplineConstruction` наследуется от следующей цепочки классов:
```
System.Object 
  TFlex.Model.ModelObject 
    TFlex.Model.Model2D.Object2D 
      TFlex.Model.Model2D.Construction 
        TFlex.Model.Model2D.SplineConstruction
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

3. **Используйте соответствующие методы** для создания нужного типа сплайна:
   - Устанавливайте `StartTangentNode` для задания начальной точки
   - Используйте `AddPoint()` для добавления точек
   - Устанавливайте свойства `Closed` и `Interpolating` по необходимости

4. **Управляйте свойствами отображения** для лучшей визуализации:
   ```csharp
   spline.Color = 255;  // Красный цвет
   spline.Layer = 2;   // Слой 2
   ```

Эти примеры охватывают основные аспекты работы с классом `SplineConstruction` в T-Flex CAD API и могут быть использованы в базе знаний для RAG-системы.
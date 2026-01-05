# Продвинутые примеры использования класса ConstructionOutline в T-Flex CAD API

## Работа с различными типами геометрии

### Создание сложных геометрических фигур

```csharp
public static void CreateComplexShape()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание сложной фигуры");
    
    // Создание узлов для многоугольника
    FreeNode fn1 = new FreeNode(document, 50, 50);
    FreeNode fn2 = new FreeNode(document, 150, 50);
    FreeNode fn3 = new FreeNode(document, 200, 100);
    FreeNode fn4 = new FreeNode(document, 150, 150);
    FreeNode fn5 = new FreeNode(document, 50, 150);
    FreeNode fn6 = new FreeNode(document, 0, 100);
    
    // Создание линий изображения
    ConstructionOutline line1 = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline line2 = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline line3 = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline line4 = new ConstructionOutline(document, fn4, fn5);
    ConstructionOutline line5 = new ConstructionOutline(document, fn5, fn6);
    ConstructionOutline line6 = new ConstructionOutline(document, fn6, fn1);
    
    // Настройка свойств линий
    line1.Color = 255; // Красный
    line2.Color = 65280; // Зеленый
    line3.Color = 16711680; // Синий
    line4.Style = LineStyle.Dash;
    line5.Style = LineStyle.DashDot;
    line6.LineWidth = 0.5;
    
    document.EndChanges();
}
```

### Создание параметрической фигуры

```csharp
public static void CreateParametricShape(double width, double height, double posX, double posY)
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание параметрической фигуры");
    
    // Вычисление координат углов
    double x1 = posX;
    double y1 = posY;
    double x2 = posX + width;
    double y2 = posY + height;
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, x1, y1);
    FreeNode fn2 = new FreeNode(document, x2, y1);
    FreeNode fn3 = new FreeNode(document, x2, y2);
    FreeNode fn4 = new FreeNode(document, x1, y2);
    
    // Создание линий изображения
    ConstructionOutline bottom = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline right = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline top = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline left = new ConstructionOutline(document, fn4, fn1);
    
    // Настройка свойств
    bottom.Color = 255;
    right.Color = 255;
    top.Color = 255;
    left.Color = 255;
    
    document.EndChanges();
}
```

## Интеграция с другими объектами

### Создание профиля на основе линий изображения

```csharp
public static void CreateProfileFromOutlines()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание профиля");
    
    // Создание замкнутого контура
    FreeNode fn1 = new FreeNode(document, 100, 100);
    FreeNode fn2 = new FreeNode(document, 200, 100);
    FreeNode fn3 = new FreeNode(document, 200, 200);
    FreeNode fn4 = new FreeNode(document, 100, 200);
    
    ConstructionOutline line1 = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline line2 = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline line3 = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline line4 = new ConstructionOutline(document, fn4, fn1);
    
    // Создание рабочей плоскости
    StandardWorkplane workplane = new StandardWorkplane(document, StandardWorkplane.StandardType.Front);
    
    // Создание профиля
    SketchProfile profile = new SketchProfile(document);
    profile.WorkSurface = workplane;
    
    document.EndChanges();
}
```

### Создание массива линий изображения

```csharp
public static void CreateLineArray(int count, double spacing)
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание массива линий");
    
    for (int i = 0; i < count; i++)
    {
        double y = 100 + i * spacing;
        FreeNode fn1 = new FreeNode(document, 50, y);
        FreeNode fn2 = new FreeNode(document, 150, y);
        ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);
        
        // Различные цвета для каждой линии
        line.Color = i * 255 / count;
    }
    
    document.EndChanges();
}
```

## Работа со свойствами и методами

### Получение информации о линии изображения

```csharp
public static void AnalyzeOutline(ConstructionOutline outline)
{
    // Получение информации о линии
    Node startNode = outline.StartNode;
    Node endNode = outline.EndNode;
    
    // Получение координат узлов
    double startX = startNode.X;
    double startY = startNode.Y;
    double endX = endNode.X;
    double endY = endNode.Y;
    
    // Вычисление длины линии
    double length = Math.Sqrt(Math.Pow(endX - startX, 2) + Math.Pow(endY - startY, 2));
    
    // Получение типа геометрии
    ObjectGeometryType geometryType = outline.GeometryType;
    
    // Получение подтипа
    OutlineType subType = outline.SubType;
    
    Console.WriteLine($"Линия от ({startX}, {startY}) до ({endX}, {endY})");
    Console.WriteLine($"Длина: {length}");
    Console.WriteLine($"Тип геометрии: {geometryType}");
    Console.WriteLine($"Подтип: {subType}");
}
```

### Модификация существующих линий

```csharp
public static void ModifyExistingOutline(ConstructionOutline outline, double newX, double newY)
{
    Document document = outline.Document;
    document.BeginChanges("Модификация линии");
    
    // Получение конечного узла
    Node endNode = outline.EndNode;
    
    // Изменение координат узла
    endNode.X = newX;
    endNode.Y = newY;
    
    // Обновление линии
    outline.EndNode = endNode;
    
    document.EndChanges();
}
```

## Работа с событиями и обратными связями

### Создание интерактивной линии

```csharp
public static void CreateInteractiveLine()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание интерактивной линии");
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 100, 100);
    FreeNode fn2 = new FreeNode(document, 200, 200);
    
    // Создание линии изображения
    ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);
    
    // Настройка свойств для интерактивности
    line.Color = 16711680; // Синий
    line.Style = LineStyle.Solid;
    line.LineWidth = 0.3;
    
    // Подписка на события (если доступно в API)
    // line.Changed += OnLineChanged;
    
    document.EndChanges();
}

// Обработчик события изменения линии
private static void OnLineChanged(object sender, EventArgs e)
{
    ConstructionOutline line = sender as ConstructionOutline;
    if (line != null)
    {
        // Обработка изменения линии
        Console.WriteLine("Линия была изменена");
    }
}
```

## Практические примеры использования

### Создание размерной сетки

```csharp
public static void CreateDimensionGrid(double width, double height, double spacing)
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание размерной сетки");
    
    // Создание горизонтальных линий
    int horizontalCount = (int)(height / spacing) + 1;
    for (int i = 0; i < horizontalCount; i++)
    {
        double y = i * spacing;
        FreeNode fn1 = new FreeNode(document, 0, y);
        FreeNode fn2 = new FreeNode(document, width, y);
        ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);
        line.Color = 12632256; // Серый
        line.Style = LineStyle.Dash;
    }
    
    // Создание вертикальных линий
    int verticalCount = (int)(width / spacing) + 1;
    for (int i = 0; i < verticalCount; i++)
    {
        double x = i * spacing;
        FreeNode fn1 = new FreeNode(document, x, 0);
        FreeNode fn2 = new FreeNode(document, x, height);
        ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);
        line.Color = 12632256; // Серый
        line.Style = LineStyle.Dash;
    }
    
    document.EndChanges();
}
```

### Создание технического чертежа

```csharp
public static void CreateTechnicalDrawing()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание технического чертежа");
    
    // Создание рамки чертежа
    CreateDrawingFrame(document, 0, 0, 200, 150);
    
    // Создание основной фигуры
    CreateMainShape(document, 50, 50, 100, 80);
    
    // Создание размеров
    CreateDimensions(document, 50, 50, 100, 80);
    
    document.EndChanges();
}

private static void CreateDrawingFrame(Document document, double x, double y, double width, double height)
{
    FreeNode fn1 = new FreeNode(document, x, y);
    FreeNode fn2 = new FreeNode(document, x + width, y);
    FreeNode fn3 = new FreeNode(document, x + width, y + height);
    FreeNode fn4 = new FreeNode(document, x, y + height);
    
    ConstructionOutline bottom = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline right = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline top = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline left = new ConstructionOutline(document, fn4, fn1);
    
    // Установка свойств рамки
    bottom.LineWidth = 0.5;
    right.LineWidth = 0.5;
    top.LineWidth = 0.5;
    left.LineWidth = 0.5;
}

private static void CreateMainShape(Document document, double x, double y, double width, double height)
{
    FreeNode fn1 = new FreeNode(document, x, y);
    FreeNode fn2 = new FreeNode(document, x + width, y);
    FreeNode fn3 = new FreeNode(document, x + width, y + height);
    FreeNode fn4 = new FreeNode(document, x, y + height);
    
    ConstructionOutline bottom = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline right = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline top = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline left = new ConstructionOutline(document, fn4, fn1);
}

private static void CreateDimensions(Document document, double x, double y, double width, double height)
{
    // Создание размерных линий
    // ... (реализация зависит от доступных классов в API)
}
```

## Оптимизация и производительность

### Создание множества линий эффективно

```csharp
public static void CreateMultipleOutlinesEfficiently(int count)
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание множества линий");
    
    // Предварительное создание узлов для повышения производительности
    List<FreeNode> nodes = new List<FreeNode>();
    for (int i = 0; i < count + 1; i++)
    {
        FreeNode node = new FreeNode(document, i * 10, 100);
        nodes.Add(node);
    }
    
    // Создание линий между узлами
    for (int i = 0; i < count; i++)
    {
        ConstructionOutline line = new ConstructionOutline(document, nodes[i], nodes[i + 1]);
        line.Color = i % 2 == 0 ? 255 : 16711680; // Чередование красного и синего
    }
    
    document.EndChanges();
}
```

## Обработка ошибок и исключений

```csharp
public static void SafeCreateOutline(Document document, double x1, double y1, double x2, double y2)
{
    try
    {
        document.BeginChanges("Безопасное создание линии");
        
        // Проверка корректности координат
        if (double.IsNaN(x1) || double.IsNaN(y1) || double.IsNaN(x2) || double.IsNaN(y2))
        {
            throw new ArgumentException("Координаты не могут быть NaN");
        }
        
        // Создание узлов
        FreeNode fn1 = new FreeNode(document, x1, y1);
        FreeNode fn2 = new FreeNode(document, x2, y2);
        
        // Проверка, что узлы не совпадают
        if (Math.Abs(x1 - x2) < 0.001 && Math.Abs(y1 - y2) < 0.001)
        {
            Console.WriteLine("Предупреждение: Узлы совпадают, линия не будет видна");
        }
        
        // Создание линии изображения
        ConstructionOutline outline = new ConstructionOutline(document, fn1, fn2);
        
        document.EndChanges();
    }
    catch (Exception ex)
    {
        document.CancelChanges();
        Console.WriteLine($"Ошибка при создании линии: {ex.Message}");
        throw;
    }
}
```

Эти продвинутые примеры демонстрируют различные аспекты работы с классом `ConstructionOutline`, включая создание сложных геометрических фигур, интеграцию с другими объектами, работу со свойствами и методами, а также практические рекомендации по оптимизации и обработке ошибок.
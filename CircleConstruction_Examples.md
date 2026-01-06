# Примеры использования класса CircleConstruction в T-Flex CAD API

## Описание класса

Класс `CircleConstruction` представляет собой линию построения в виде окружности в 2D-пространстве. Он наследуется от класса `Construction` и предоставляет функциональность для создания различных типов окружностей построения.

## Конструкторы

### 1. CircleConstruction(Document)

Конструктор по умолчанию для создания окружности построения.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание окружности построения");

// Создание окружности построения
CircleConstruction circle = new CircleConstruction(document);

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. CircleConstruction(Document, Point, Construction, Construction)

Конструктор для создания окружности построения с параметрами.

## Основные методы создания окружностей

### 1. Создание окружности с центром и радиусом
```csharp
public static void CreateCircleWithCenterAndRadius()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание окружности с центром и радиусом");
    
    // Создание центрального узла
    FreeNode center = new FreeNode(document, 25, 25);
    
    // Создание окружности построения
    CircleConstruction circle = new CircleConstruction(document);
    circle.SetCenterAndRadius(center, 20); // Центр и радиус
    
    document.EndChanges();
}
```

### 2. Создание окружности через три узла
```csharp
public static void CreateCircleThroughThreeNodes()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание окружности через три узла");
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 10, 10);
    FreeNode fn2 = new FreeNode(document, 50, 10);
    FreeNode fn3 = new FreeNode(document, 30, 40);
    
    // Создание окружности построения
    CircleConstruction circle = new CircleConstruction(document);
    circle.SetThreeNodes(fn1, fn2, fn3);
    
    document.EndChanges();
}
```

### 3. Создание окружности касательной к двум прямым
```csharp
public static void CreateCircleTangentToTwoLines()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание окружности касательной к двум прямым");
    
    // Создание прямых
    FreeNode line1Node1 = new FreeNode(document, 10, 10);
    FreeNode line1Node2 = new FreeNode(document, 10, 50);
    LineConstruction line1 = new LineConstruction(document);
    line1.SetThroughNodes(line1Node1, line1Node2);
    
    FreeNode line2Node1 = new FreeNode(document, 0, 40);
    FreeNode line2Node2 = new FreeNode(document, 50, 40);
    LineConstruction line2 = new LineConstruction(document);
    line2.SetThroughNodes(line2Node1, line2Node2);
    
    // Создание окружности построения
    CircleConstruction circle = new CircleConstruction(document);
    int radius = 20; // Радиус окружности
    int variant = 2; // Номер варианта касания
    circle.SetTangentToTwoLines(line1, line2, radius, variant);
    
    document.EndChanges();
}
```

## Свойства класса

### Основные свойства:

1. **SubType** - Подтип линии построения (всегда CircleConstruction)
2. **GeometryType** - Тип геометрии линии построения (окружность)
3. **ConstructionGeometry** - Геометрия линии построения
4. **CircleConstructionGeometry** - Геометрия линии построения (окружности)
5. **CircleType** - Тип привязки окружности

### Пример работы со свойствами:
```csharp
public static void WorkWithCircleProperties()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Работа со свойствами окружности");
    
    FreeNode center = new FreeNode(document, 25, 25);
    CircleConstruction circle = new CircleConstruction(document);
    circle.SetCenterAndRadius(center, 20);
    
    // Получение свойств
    ConstructionType subType = circle.SubType;  // CircleConstruction
    ObjectGeometryType geomType = circle.GeometryType; // Circle
    
    // Установка свойств отображения
    circle.Color = 255;    // Красный цвет
    circle.Layer = 2;      // Слой 2
    circle.Visible = true; // Видимость
    
    document.EndChanges();
}
```

## Примеры использования в контексте других объектов

### Создание окружности касательной к прямой:
```csharp
public static void CreateCircleTangentToLine()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание окружности касательной к прямой");
    
    // Создание прямой
    FreeNode lineNode1 = new FreeNode(document, 10, 10);
    FreeNode lineNode2 = new FreeNode(document, 50, 10);
    LineConstruction line = new LineConstruction(document);
    line.SetThroughNodes(lineNode1, lineNode2);
    
    // Создание узла
    FreeNode node = new FreeNode(document, 30, 30);
    
    // Создание окружности построения
    CircleConstruction circle = new CircleConstruction(document);
    circle.SetTangentToLineAndNode(line, node);
    
    document.EndChanges();
}
```

### Создание окружности касательной к другой окружности:
```csharp
public static void CreateCircleTangentToCircle()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание окружности касательной к другой окружности");
    
    // Создание первой окружности
    FreeNode center1 = new FreeNode(document, 20, 20);
    CircleConstruction circle1 = new CircleConstruction(document);
    circle1.SetCenterAndRadius(center1, 15);
    
    // Создание узла
    FreeNode node = new FreeNode(document, 50, 50);
    
    // Создание второй окружности построения
    CircleConstruction circle2 = new CircleConstruction(document);
    circle2.SetTangentToCircleAndNode(circle1, node);
    
    document.EndChanges();
}
```

## Типы линий построения в T-Flex CAD API

Класс `CircleConstruction` является одним из основных типов линий построения в T-Flex CAD API:

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

Класс `CircleConstruction` наследуется от следующей цепочки классов:
```
System.Object 
  TFlex.Model.ModelObject 
    TFlex.Model.Model2D.Object2D 
      TFlex.Model.Model2D.Construction 
        TFlex.Model.Model2D.CircleConstruction
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

3. **Используйте соответствующие методы** для создания нужного типа окружности:
   - `SetCenterAndRadius()` для окружности с центром и радиусом
   - `SetThreeNodes()` для окружности через три узла
   - `SetTangentToTwoLines()` для окружности касательной к двум прямым

4. **Управляйте свойствами отображения** для лучшей визуализации:
   ```csharp
   circle.Color = 255;  // Красный цвет
   circle.Layer = 2;   // Слой 2
   ```

Эти примеры охватывают основные аспекты работы с классом `CircleConstruction` в T-Flex CAD API и могут быть использованы в базе знаний для RAG-системы.
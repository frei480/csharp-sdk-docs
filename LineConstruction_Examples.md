# Примеры использования класса LineConstruction в T-Flex CAD API

## Описание класса

Класс `LineConstruction` представляет собой линию построения в виде прямой линии в 2D-пространстве. Он наследуется от класса `Construction` и предоставляет функциональность для создания различных типов прямых линий построения.

## Конструкторы

### 1. LineConstruction(Document)

Конструктор по умолчанию для создания линии построения.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание линии построения");

// Создание линии построения
LineConstruction line = new LineConstruction(document);

// Закрытие блока изменений документа
document.EndChanges();
```

## Основные методы создания прямых

### 1. Создание прямой через два узла
```csharp
public static void CreateLineThroughNodes()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание прямой через узлы");
    
    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 10, 10);
    FreeNode fn2 = new FreeNode(document, 50, 10);
    
    // Создание линии построения
    LineConstruction lc = new LineConstruction(document);
    lc.SetThroughNodes(fn1, fn2);
    
    document.EndChanges();
}
```

### 2. Создание горизонтальной прямой
```csharp
public static void CreateHorizontalLine()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание горизонтальной прямой");
    
    LineConstruction lc = new LineConstruction(document);
    lc.SetHorizontal();
    
    document.EndChanges();
}
```

### 3. Создание горизонтальной прямой через узел
```csharp
public static void CreateHorizontalLineThroughNode()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание горизонтальной прямой через узел");
    
    FreeNode node = new FreeNode(document, 25, 25);
    LineConstruction lc = new LineConstruction(document);
    lc.SetHorizontalThroughNode(node);
    
    document.EndChanges();
}
```

### 4. Создание вертикальной прямой
```csharp
public static void CreateVerticalLine()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание вертикальной прямой");
    
    LineConstruction lc = new LineConstruction(document);
    lc.SetVertical();
    
    document.EndChanges();
}
```

### 5. Создание вертикальной прямой через узел
```csharp
public static void CreateVerticalLineThroughNode()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание вертикальной прямой через узел");
    
    FreeNode node = new FreeNode(document, 25, 25);
    LineConstruction lc = new LineConstruction(document);
    lc.SetVerticalThroughNode(node);
    
    document.EndChanges();
}
```

## Свойства класса

### Основные свойства:

1. **SubType** - Подтип линии построения (всегда LineConstruction)
2. **GeometryType** - Тип геометрии линии построения
3. **ConstructionGeometry** - Геометрия линии построения
4. **LineConstructionGeometry** - Геометрия линии построения (прямой)
5. **LineType** - Тип привязки прямой
6. **LineView** - Вид прямой

### Пример работы со свойствами:
```csharp
public static void WorkWithLineProperties()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Работа со свойствами линии");
    
    LineConstruction lc = new LineConstruction(document);
    lc.SetHorizontal();
    
    // Получение свойств
    ConstructionType subType = lc.SubType;  // LineConstruction
    ObjectGeometryType geomType = lc.GeometryType;
    
    // Установка свойств отображения
    lc.Color = 255;    // Красный цвет
    lc.Layer = 2;      // Слой 2
    lc.Visible = true; // Видимость
    
    document.EndChanges();
}
```

## Примеры использования в контексте других объектов

### Создание параллельной прямой:
```csharp
public static void CreateParallelLine()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание параллельной прямой");
    
    // Создание исходной прямой
    FreeNode fn1 = new FreeNode(document, 10, 10);
    FreeNode fn2 = new FreeNode(document, 50, 10);
    LineConstruction sourceLine = new LineConstruction(document);
    sourceLine.SetThroughNodes(fn1, fn2);
    
    // Создание параллельной прямой через узел
    FreeNode node = new FreeNode(document, 25, 25);
    LineConstruction parallelLine = new LineConstruction(document);
    parallelLine.SetParallelThroughNode(sourceLine, node);
    
    document.EndChanges();
}
```

### Создание перпендикулярной прямой:
```csharp
public static void CreatePerpendicularLine()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание перпендикулярной прямой");
    
    // Создание исходной прямой
    FreeNode fn1 = new FreeNode(document, 10, 10);
    FreeNode fn2 = new FreeNode(document, 50, 10);
    LineConstruction sourceLine = new LineConstruction(document);
    sourceLine.SetThroughNodes(fn1, fn2);
    
    // Создание перпендикулярной прямой через узел
    FreeNode node = new FreeNode(document, 25, 25);
    LineConstruction perpendicularLine = new LineConstruction(document);
    perpendicularLine.SetPerpendicularThroughNode(sourceLine, node);
    
    document.EndChanges();
}
```

## Типы линий построения в T-Flex CAD API

Класс `LineConstruction` является одним из основных типов линий построения в T-Flex CAD API:

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

Класс `LineConstruction` наследуется от следующей цепочки классов:
```
System.Object 
  TFlex.Model.ModelObject 
    TFlex.Model.Model2D.Object2D 
      TFlex.Model.Model2D.Construction 
        TFlex.Model.Model2D.LineConstruction
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

3. **Используйте соответствующие методы** для создания нужного типа прямой:
   - `SetThroughNodes()` для прямой через два узла
   - `SetHorizontal()` для горизонтальной прямой
   - `SetVertical()` для вертикальной прямой
   - `SetParallelThroughNode()` для параллельной прямой

4. **Управляйте свойствами отображения** для лучшей визуализации:
   ```csharp
   line.Color = 255;  // Красный цвет
   line.Layer = 2;   // Слой 2
   ```

Эти примеры охватывают основные аспекты работы с классом `LineConstruction` в T-Flex CAD API и могут быть использованы в базе знаний для RAG-системы.
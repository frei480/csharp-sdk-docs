# Примеры использования класса ConstructionOutline в T-Flex CAD API

## Описание класса

Класс `ConstructionOutline` представляет собой линию изображения, основанную на узлах и линиях построения. Он наследуется от класса `Outline` и предоставляет функциональность для создания линий изображения, которые могут быть основаны на узлах или линиях построения.

## Конструкторы

### 1. ConstructionOutline(Document, Node, Node)

Создает линию изображения между двумя узлами.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание линии изображения");

// Создание узлов
FreeNode fn1 = new FreeNode(document, 400, 320);
FreeNode fn2 = new FreeNode(document, 400, 420);

// Создание линии изображения между двумя узлами
ConstructionOutline conOutline = new ConstructionOutline(document, fn1, fn2);

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. ConstructionOutline(Document, Construction)

Создает линию изображения на основе линии построения.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание линии изображения по линии построения");

// Создание линии построения (например, окружности)
FreeNode fnCenter = new FreeNode(document, 200, 370);
int radius = 50;
CircleConstruction circleConstruction = new CircleConstruction(document, fnCenter, radius);

// Создание линии изображения на основе линии построения
ConstructionOutline conOutline = new ConstructionOutline(document, circleConstruction);

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. ConstructionOutline(Document, Node, Node, Construction)

Создает линию изображения между двумя узлами с использованием линии построения.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание линии изображения с линией построения");

// Создание узлов
FreeNode fn1 = new FreeNode(document, 400, 320);
FreeNode fn2 = new FreeNode(document, 400, 420);

// Создание линии построения (например, дуги)
// ... (создание дуги)

// Создание линии изображения между узлами с использованием линии построения
ConstructionOutline conOutline = new ConstructionOutline(document, fn1, fn2, arcConstruction);

// Закрытие блока изменений документа
document.EndChanges();
```

## Свойства класса

### Основные свойства:

1. **StartNode** - Начальный узел линии изображения
2. **EndNode** - Конечный узел линии изображения
3. **Construction** - Линия построения, по которой проходит линия изображения
4. **AnchorNode** - Узел привязки (для дуг и эллипсов)
5. **GeometryType** - Тип геометрии линии изображения
6. **SubType** - Подтип линии изображения

### Пример работы со свойствами:
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
document.BeginChanges("Работа со свойствами линии изображения");

// Создание узлов
FreeNode fn1 = new FreeNode(document, 100, 100);
FreeNode fn2 = new FreeNode(document, 200, 100);

// Создание линии изображения
ConstructionOutline newOutline = new ConstructionOutline(document, fn1, fn2);

// Работа со свойствами
Node startNode = newOutline.StartNode;  // Получение начального узла
Node endNode = newOutline.EndNode;      // Получение конечного узла

// Изменение свойств линии изображения
newOutline.Color = 255;                 // Установка цвета (красный)
newOutline.Style = LineStyle.Solid;     // Установка стиля линии
newOutline.LineWidth = 0.5;            // Установка толщины линии

document.EndChanges();
```

## Примеры использования в контексте других объектов

### Создание треугольника из линий изображения:
```csharp
public static void CreateTriangle()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание треугольника");

    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 10, 10);
    FreeNode fn2 = new FreeNode(document, 40, 30);
    FreeNode fn3 = new FreeNode(document, 70, 10);

    // Создание линий изображения между узлами
    ConstructionOutline l1 = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline l2 = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline l3 = new ConstructionOutline(document, fn3, fn1);

    document.EndChanges();
}
```

### Создание линии изображения как оси для других объектов:
```csharp
public static void CreateAxisOutline()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание оси");

    // Создание окружности
    FreeNode fnCenter = new FreeNode(document, 200, 370);
    int radius = 50;
    CircleOutline co = new CircleOutline(document, fnCenter, radius);
    
    // Создание центральной оси окружности
    CenterAxisOutline cao = new CenterAxisOutline(document, co, false);
    
    // Создание прямой линии
    FreeNode fn1 = new FreeNode(document, 400, 320);
    FreeNode fn2 = new FreeNode(document, 400, 420);
    ConstructionOutline conOutline = new ConstructionOutline(document, fn1, fn2);
    
    // Создание оси двух линий изображения
    AxisOutline axOutline = new AxisOutline(document, cao, conOutline);

    document.EndChanges();
}
```

## Типы геометрии и подтипы

Класс `ConstructionOutline` может представлять различные типы геометрии:
- Прямые линии (отрезки)
- Дуги окружностей
- Эллиптические дуги

Подтипы определяются перечислением `OutlineType`, где `ConstructionOutline` имеет значение `ConstructionOutline`.

## Наследование

Класс `ConstructionOutline` наследуется от следующей цепочки классов:
```
System.Object 
  TFlex.Model.ModelObject 
    TFlex.Model.Model2D.Object2D 
      TFlex.Model.Model2D.Outline 
        TFlex.Model.Model2D.ConstructionOutline
```

Это означает, что он наследует все свойства и методы этих классов, включая:
- Свойства отображения (цвет, стиль, толщина линии)
- Методы работы с геометрией
- Методы преобразования (перемещение, поворот)
- Свойства видимости и слоя

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

3. **Используйте соответствующие типы узлов** в зависимости от задачи:
   - `FreeNode` для свободных узлов
   - `ConstructionNode` для узлов на линиях построения
   - `OutlineNode` для узлов на линиях изображения

4. **Управляйте свойствами отображения** для лучшей визуализации:
   ```csharp
   outline.Color = 255;        // Красный цвет
   outline.Style = LineStyle.Dash;  // Пунктирная линия
   outline.LineWidth = 0.3;   // Толщина линии
   ```

Эти примеры охватывают основные аспекты работы с классом `ConstructionOutline` в T-Flex CAD API и могут быть использованы в базе знаний для RAG-системы.
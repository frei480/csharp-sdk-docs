# Шпаргалка по классу ConstructionOutline в T-Flex CAD API

## Основная информация
- **Класс**: `ConstructionOutline`
- **Назначение**: Линия изображения, основанная на узлах и линиях построения
- **Пространство имен**: `TFlex.Model.Model2D`
- **Базовый класс**: `Outline`

## Конструкторы

### 1. По двум узлам
```csharp
ConstructionOutline(Document document, Node startNode, Node endNode)
```
**Пример:**
```csharp
FreeNode fn1 = new FreeNode(document, 0, 0);
FreeNode fn2 = new FreeNode(document, 100, 100);
ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);
```

### 2. По линии построения
```csharp
ConstructionOutline(Document document, Construction srcConstruction)
```
**Пример:**
```csharp
CircleConstruction circle = new CircleConstruction(document, centerNode, 50);
ConstructionOutline outline = new ConstructionOutline(document, circle);
```

### 3. По узлам и линии построения
```csharp
ConstructionOutline(Document document, Node startNode, Node endNode, Construction srcConstruction)
```

## Основные свойства

| Свойство | Тип | Описание |
|----------|-----|----------|
| `StartNode` | `Node` | Начальный узел |
| `EndNode` | `Node` | Конечный узел |
| `Construction` | `Construction` | Линия построения |
| `AnchorNode` | `Node` | Узел привязки |
| `GeometryType` | `ObjectGeometryType` | Тип геометрии |
| `SubType` | `OutlineType` | Подтип (ConstructionOutline) |

## Свойства отображения

| Свойство | Тип | Описание |
|----------|-----|----------|
| `Color` | `int` | Цвет линии (RGB) |
| `Style` | `LineStyle` | Стиль линии |
| `LineWidth` | `double` | Толщина линии |
| `Visible` | `bool` | Видимость |
| `Layer` | `Layer` | Слой |

## Часто используемые методы (унаследованные)

| Метод | Описание |
|-------|----------|
| `Geometry` | Получение геометрии с масштабом |
| `ModelGeometry` | Получение геометрии без масштаба |
| `Transform(Matrix2D)` | Применение преобразования |
| `Translate(Vector2D)` | Сдвиг объекта |
| `SetDefaults()` | Установка параметров по умолчанию |

## Примеры использования

### Создание простой линии
```csharp
Document document = TFlex.Application.ActiveDocument;
document.BeginChanges("Создание линии");

FreeNode start = new FreeNode(document, 50, 50);
FreeNode end = new FreeNode(document, 150, 150);
ConstructionOutline line = new ConstructionOutline(document, start, end);

line.Color = 255; // Красный
line.Style = LineStyle.Solid;
line.LineWidth = 0.3;

document.EndChanges();
```

### Создание прямоугольника
```csharp
document.BeginChanges("Создание прямоугольника");

FreeNode p1 = new FreeNode(document, 0, 0);
FreeNode p2 = new FreeNode(document, 100, 0);
FreeNode p3 = new FreeNode(document, 100, 50);
FreeNode p4 = new FreeNode(document, 0, 50);

ConstructionOutline bottom = new ConstructionOutline(document, p1, p2);
ConstructionOutline right = new ConstructionOutline(document, p2, p3);
ConstructionOutline top = new ConstructionOutline(document, p3, p4);
ConstructionOutline left = new ConstructionOutline(document, p4, p1);

document.EndChanges();
```

### Работа со свойствами
```csharp
// Цвета
outline.Color = 255;        // Красный
outline.Color = 65280;      // Зеленый
outline.Color = 16711680;    // Синий

// Стили линий
outline.Style = LineStyle.Solid;      // Сплошная
outline.Style = LineStyle.Dash;        // Пунктир
outline.Style = LineStyle.DashDot;     // Штрихпунктир

// Толщина
outline.LineWidth = 0.1;  // Тонкая
outline.LineWidth = 0.5;  // Толстая
```

## Рекомендации

### Обязательно используйте:
```csharp
document.BeginChanges("Описание");
// Ваши операции
document.EndChanges();
```

### Проверяйте документ:
```csharp
if (TFlex.Application.ActiveDocument != null)
{
    Document document = TFlex.Application.ActiveDocument;
    // Работа с документом
}
```

### Обработка ошибок:
```csharp
try
{
    document.BeginChanges("Операция");
    // Операции
    document.EndChanges();
}
catch (Exception ex)
{
    document.CancelChanges();
    // Обработка ошибки
}
```

## Частые ошибки

1. ❌ Отсутствие блоков изменений
2. ❌ Некорректные координаты (NaN, Infinity)
3. ❌ Совпадающие узлы
4. ❌ Неправильное использование линий построения

## Полезные ссылки

- `Node` - узлы
- `Construction` - линии построения
- `Outline` - базовый класс линий
- `LineStyle` - стили линий
- `ObjectGeometryType` - типы геометрии

---
*Шпаргалка создана на основе документации T-Flex CAD API*
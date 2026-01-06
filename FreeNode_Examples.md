# Примеры использования класса FreeNode в T-Flex CAD API

## Описание класса

Класс `FreeNode` представляет собой узел с абсолютными координатами в системе координат модели. Он наследуется от класса `Node` и предоставляет функциональность для создания узлов, которые не зависят от других объектов и имеют фиксированные координаты.

## Конструкторы

### 1. FreeNode(Document)

Конструктор по умолчанию. Координаты установлены в значение 0,0.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание узла по умолчанию");

// Создание узла с координатами (0,0)
FreeNode defaultNode = new FreeNode(document);

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. FreeNode(Document, Parameter, Parameter)

Конструктор, задающий координаты x,y в системе координат модели, без учёта масштаба текущей страницы.

**Пример:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
// Открытие блока изменений документа
document.BeginChanges("Создание узла с координатами");

// Создание узла с заданными координатами
FreeNode fn = new FreeNode(document, 100, 200);

// Закрытие блока изменений документа
document.EndChanges();
```

## Свойства класса

### Основные свойства:

1. **X** - Значение координаты X узла
2. **Y** - Значение координаты Y узла
3. **AbsX** - Координата X в системе координат модели (без учёта масштаба страницы)
4. **AbsY** - Координата Y в системе координат модели (без учёта масштаба страницы)
5. **Coordinates** - Координаты узла в системе координат модели
6. **Color** - Цвет объекта
7. **Layer** - Слой, на котором размещается объект
8. **Level** - Уровень объекта

### Пример работы со свойствами:
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;
document.BeginChanges("Работа со свойствами узла");

// Создание узла
FreeNode fn = new FreeNode(document, 150, 150);

// Получение значений координат
double xCoord = fn.X.Value;  // Получение значения координаты X
double yCoord = fn.Y.Value;  // Получение значения координаты Y

// Изменение координат узла
fn.X.Value = 200;  // Изменение координаты X
fn.Y.Value = 250;  // Изменение координаты Y

// Изменение свойств отображения
fn.Color = 255;    // Установка красного цвета
fn.Layer = 1;      // Установка слоя 1

document.EndChanges();
```

## Примеры использования в контексте других объектов

### Создание линии изображения между двумя узлами:
```csharp
public static void CreateLineBetweenNodes()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание линии между узлами");

    // Создание узлов
    FreeNode fn1 = new FreeNode(document, 100, 100);
    FreeNode fn2 = new FreeNode(document, 200, 200);

    // Создание линии изображения между узлами
    ConstructionOutline line = new ConstructionOutline(document, fn1, fn2);

    document.EndChanges();
}
```

### Создание окружности с центром в узле:
```csharp
public static void CreateCircleWithCenterNode()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание окружности");

    // Создание узла для центра окружности
    FreeNode centerNode = new FreeNode(document, 150, 150);

    // Создание окружности построения
    int radius = 50;
    CircleConstruction circle = new CircleConstruction(document, centerNode, radius);

    document.EndChanges();
}
```

### Создание прямоугольника из узлов:
```csharp
public static void CreateRectangleFromNodes()
{
    Document document = TFlex.Application.ActiveDocument;
    document.BeginChanges("Создание прямоугольника");

    // Создание узлов для углов прямоугольника
    FreeNode fn1 = new FreeNode(document, 100, 100);  // Левый нижний угол
    FreeNode fn2 = new FreeNode(document, 200, 100);  // Правый нижний угол
    FreeNode fn3 = new FreeNode(document, 200, 200);  // Правый верхний угол
    FreeNode fn4 = new FreeNode(document, 100, 200);  // Левый верхний угол

    // Создание линий изображения
    ConstructionOutline line1 = new ConstructionOutline(document, fn1, fn2);
    ConstructionOutline line2 = new ConstructionOutline(document, fn2, fn3);
    ConstructionOutline line3 = new ConstructionOutline(document, fn3, fn4);
    ConstructionOutline line4 = new ConstructionOutline(document, fn4, fn1);

    document.EndChanges();
}
```

## Типы узлов в T-Flex CAD API

Класс `FreeNode` является одним из трех основных типов узлов в T-Flex CAD API:

1. **FreeNode** - Узел с абсолютными координатами
2. **ConstructionNode** - Узел на линии построения
3. **OutlineNode** - Узел на линии изображения

## Наследование

Класс `FreeNode` наследуется от следующей цепочки классов:
```
System.Object 
  TFlex.Model.ModelObject 
    TFlex.Model.Model2D.Object2D 
      TFlex.Model.Model2D.Node 
        TFlex.Model.Model2D.FreeNode
```

Это означает, что он наследует все свойства и методы этих классов, включая:
- Свойства отображения (цвет, слой, уровень)
- Свойства координат
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

3. **Используйте соответствующие типы узлов** в зависимости от задачи:
   - `FreeNode` для свободных узлов с фиксированными координатами
   - `ConstructionNode` для узлов на линиях построения
   - `OutlineNode` для узлов на линиях изображения

4. **Управляйте свойствами отображения** для лучшей визуализации:
   ```csharp
   node.Color = 255;  // Красный цвет
   node.Layer = 2;    // Слой 2
   ```

Эти примеры охватывают основные аспекты работы с классом `FreeNode` в T-Flex CAD API и могут быть использованы в базе знаний для RAG-системы.
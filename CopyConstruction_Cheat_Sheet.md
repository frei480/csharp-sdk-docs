# CopyConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
CopyConstruction представляет собой копию линии построения в T-Flex CAD API. Это геометрический элемент для создания копий других геометрических объектов с применением трансформаций.

## Основные свойства
- `Source` - Исходная линия построения (Construction)
- `Matrix` - Матрица трансформации (Matrix3D)
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Конструкторы
```csharp
// Создание пустой копии линии построения
CopyConstruction copy = new CopyConstruction(document);
```

## Основные методы
- `SetSource(Construction source)` - Установка исходного объекта
- `SetMatrix(Matrix3D matrix)` - Установка матрицы трансформации
- `SetTranslation(double dx, double dy, double dz)` - Установка трансляции
- `SetRotation(double angle, double axisX, double axisY, double axisZ)` - Установка вращения
- `SetScale(double scaleX, double scaleY, double scaleZ)` - Установка масштабирования
- `GetTransformedGeometry()` - Получение трансформированной геометрии

## Примеры использования

### Базовое использование
```csharp
// Создание простой копии объекта
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 50, 50), 10);

CopyConstruction copy = new CopyConstruction(document);
copy.SetSource(originalCircle);
copy.SetTranslation(30, 0, 0); // Смещение вправо на 30 единиц
copy.Color = 255; // Красный цвет
```

### Создание копии с вращением
```csharp
// Создание копии с вращением
LineConstruction originalLine = new LineConstruction(document);
originalLine.SetTwoNodes(new FreeNode(document, 40, 50), new FreeNode(document, 60, 50));

CopyConstruction rotatedCopy = new CopyConstruction(document);
rotatedCopy.SetSource(originalLine);
// Вращение на 45 градусов вокруг центра (50, 50)
rotatedCopy.SetRotation(Math.PI / 4, 50, 50, 0);
rotatedCopy.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание массива копий
```csharp
// Создание массива копий
CircleConstruction originalCircle = new CircleConstruction(document);
originalCircle.SetCenterAndRadius(new FreeNode(document, 30, 50), 5);

int arrayCount = 5;
CopyConstruction[] copies = new CopyConstruction[arrayCount];

for (int i = 0; i < arrayCount; i++)
{
    copies[i] = new CopyConstruction(document);
    copies[i].SetSource(originalCircle);
    copies[i].SetTranslation(i * 15, 0, 0); // Смещение по X
    
    // Установка цвета с градиентом
    int red = (int)(255 * (double)i / (arrayCount - 1));
    int green = 255 - red;
    int blue = 128;
    copies[i].Color = (red << 16) | (green << 8) | blue;
}
```

### Создание копий с геометрическими трансформациями
```csharp
// Создание копий с различными трансформациями
EllipseConstruction originalEllipse = new EllipseConstruction(document);
originalEllipse.SetCenterAndRadii(new FreeNode(document, 50, 50), 15, 10);

int transformCount = 4;
CopyConstruction[] transformedCopies = new CopyConstruction[transformCount];

for (int i = 0; i < transformCount; i++)
{
    transformedCopies[i] = new CopyConstruction(document);
    transformedCopies[i].SetSource(originalEllipse);
    
    switch (i)
    {
        case 0: // Трансляция
            transformedCopies[i].SetTranslation(40, 0, 0);
            break;
        case 1: // Вращение
            transformedCopies[i].SetRotation(Math.PI / 2, 50, 50, 0);
            break;
        case 2: // Масштабирование
            // В реальной реализации потребуется способ применения масштабирования
            transformedCopies[i].SetTranslation(0, 40, 0);
            break;
        case 3: // Комбинация трансформаций
            transformedCopies[i].SetTranslation(-40, 0, 0);
            // В реальной реализации можно комбинировать трансформации
            break;
    }
    
    // Установка цвета
    transformedCopies[i].Color = 16711680; // Синий цвет
}
```

## Связанные объекты
- SymmetryConstruction - Симметричная копия линии построения
- OffsetConstruction - Смещенная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура
- Matrix3D - Трехмерная матрица трансформации

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества копий
2. Убедитесь, что исходные объекты существуют и корректны
3. Проверяйте трансформации перед применением к копиям

## Лучшие практики
1. Используйте параметризованные копии для создания динамических конструкций
2. При создании больших массивов копий используйте оптимизацию производительности
3. Используйте копии повторно при создании сложных конструкций
# FunctionConstruction - примеры использования

Класс `FunctionConstruction` представляет линию построения-функцию. Этот класс наследуется от `Construction` и предоставляет специфичные свойства и методы для создания линий построения на основе математических функций.

## Основные свойства

- `FunctionName` - Имя функции
- `FirstTerm` - Первое выражение, задающее функцию
- `SecondTerm` - Второе выражение, задающее функцию
- `Start` - Начало функции
- `End` - Окончание функции
- `OriginNode` - Начальный узел
- `DirectionNode` - Узел направления системы координат
- `Type` - Тип функции
- `NumberOfPoints` - Количество точек (при постоянном шаге полилинии)
- `ClosedSpline` - Замкнутый сплайн
- `ConvertToSpline` - Создавать сплайн по полилинии

## Примеры использования

### 1. Создание параболы

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параболы");

// Создание функции-параболы
FunctionConstruction parabola = new FunctionConstruction(document);
parabola.FunctionName = "Парабола";
parabola.FirstTerm = "#1**2"; // y = x^2
parabola.Start = -3; // Начало функции
parabola.End = 3; // Окончание функции

// Создание узлов для определения системы координат
FreeNode origin = new FreeNode(document, 50, 50); // Начало координат
FreeNode direction = new FreeNode(document, 55, 50); // Направление оси X

// Установка узлов
parabola.OriginNode = origin;
parabola.DirectionNode = direction;

// Установка типа функции
parabola.Type = FunctionConstruction.FunctionType.Plain; // Обычная функция

// Установка визуальных свойств
parabola.Color = 255; // Красный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание синусоиды

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание синусоиды");

// Создание функции-синусоиды
FunctionConstruction sine = new FunctionConstruction(document);
sine.FunctionName = "Синусоида";
sine.FirstTerm = "sin(#1)"; // y = sin(x)
sine.Start = 0; // Начало функции
sine.End = 2 * Math.PI; // Окончание функции (2π)

// Создание узлов для определения системы координат
FreeNode origin = new FreeNode(document, 30, 50); // Начало координат
FreeNode direction = new FreeNode(document, 35, 50); // Направление оси X

// Установка узлов
sine.OriginNode = origin;
sine.DirectionNode = direction;

// Установка типа функции
sine.Type = FunctionConstruction.FunctionType.Plain; // Обычная функция

// Установка визуальных свойств
sine.Color = 65280; // Зеленый цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание параметрической функции (спирали)

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание спирали");

// Создание параметрической функции-спирали
FunctionConstruction spiral = new FunctionConstruction(document);
spiral.FunctionName = "Спираль";
spiral.FirstTerm = "#1 * cos(#1)"; // x = t * cos(t)
spiral.SecondTerm = "#1 * sin(#1)"; // y = t * sin(t)
spiral.Start = 0; // Начало функции
spiral.End = 4 * Math.PI; // Окончание функции (4π)

// Создание узлов для определения системы координат
FreeNode origin = new FreeNode(document, 50, 50); // Начало координат
FreeNode direction = new FreeNode(document, 55, 50); // Направление оси X

// Установка узлов
spiral.OriginNode = origin;
spiral.DirectionNode = direction;

// Установка типа функции
spiral.Type = FunctionConstruction.FunctionType.Parametric; // Параметрическая функция

// Установка визуальных свойств
spiral.Color = 16711680; // Синий цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Создание функции с использованием сплайна

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание функции со сплайном");

// Создание функции с преобразованием в сплайн
FunctionConstruction function = new FunctionConstruction(document);
function.FunctionName = "Функция со сплайном";
function.FirstTerm = "#1**3 - 2*#1"; // y = x^3 - 2x
function.Start = -2; // Начало функции
function.End = 2; // Окончание функции

// Создание узлов для определения системы координат
FreeNode origin = new FreeNode(document, 50, 50); // Начало координат
FreeNode direction = new FreeNode(document, 55, 50); // Направление оси X

// Установка узлов
function.OriginNode = origin;
function.DirectionNode = direction;

// Установка типа функции
function.Type = FunctionConstruction.FunctionType.Plain; // Обычная функция

// Настройка параметров сплайна
function.ConvertToSpline = true; // Преобразовать в сплайн
function.SplinePoints = 20; // Количество точек сплайна

// Установка визуальных свойств
function.Color = 16711935; // Пурпурный цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Создание функции с переменным шагом

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание функции с переменным шагом");

// Создание функции с переменным шагом
FunctionConstruction function = new FunctionConstruction(document);
function.FunctionName = "Функция с переменным шагом";
function.FirstTerm = "exp(#1)"; // y = e^x
function.Start = -2; // Начало функции
function.End = 2; // Окончание функции

// Создание узлов для определения системы координат
FreeNode origin = new FreeNode(document, 30, 30); // Начало координат
FreeNode direction = new FreeNode(document, 35, 30); // Направление оси X

// Установка узлов
function.OriginNode = origin;
function.DirectionNode = direction;

// Установка типа функции
function.Type = FunctionConstruction.FunctionType.Plain; // Обычная функция

// Настройка параметров оптимизации
function.CurvatureOptimization = true; // Оптимизировать по кривизне
function.CurvatureTolerance = 0.1; // Допуск при оптимизации

// Установка визуальных свойств
function.Color = 65535; // Голубой цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Интеграция функции с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция функции с другими объектами");

// Создание функции-параболы
FunctionConstruction parabola = new FunctionConstruction(document);
parabola.FunctionName = "Парабола";
parabola.FirstTerm = "0.1 * #1**2"; // y = 0.1 * x^2
parabola.Start = -20; // Начало функции
parabola.End = 20; // Окончание функции

// Создание узлов для определения системы координат
FreeNode origin = new FreeNode(document, 50, 30); // Начало координат
FreeNode direction = new FreeNode(document, 55, 30); // Направление оси X

// Установка узлов
parabola.OriginNode = origin;
parabola.DirectionNode = direction;

// Установка типа функции
parabola.Type = FunctionConstruction.FunctionType.Plain; // Обычная функция

// Создание точек на функции для построения касательных
FreeNode point1 = new FreeNode(document, origin.X.Value + 10, origin.Y.Value + 10); // Точка на параболе
FreeNode point2 = new FreeNode(document, origin.X.Value - 10, origin.Y.Value + 10); // Другая точка на параболе

// Создание касательных к параболе в заданных точках
// (в данном примере создаем приблизительные касательные)
LineConstruction tangent1 = new LineConstruction(document);
tangent1.SetTwoNodes(new FreeNode(document, point1.X.Value - 5, point1.Y.Value - 2), 
                     new FreeNode(document, point1.X.Value + 5, point1.Y.Value + 2));

LineConstruction tangent2 = new LineConstruction(document);
tangent2.SetTwoNodes(new FreeNode(document, point2.X.Value - 5, point2.Y.Value + 2), 
                     new FreeNode(document, point2.X.Value + 5, point2.Y.Value - 2));

// Установка визуальных свойств
parabola.Color = 255; // Красный (парабола)
tangent1.Color = 65280; // Зеленый (первая касательная)
tangent2.Color = 16711680; // Синий (вторая касательная)

// Закрытие блока изменений документа
document.EndChanges();
```

## Свойства и методы

### Основные свойства:

- `FunctionName` - Имя функции
- `FirstTerm` - Первое выражение, задающее функцию
- `SecondTerm` - Второе выражение, задающее функцию
- `Start` - Начало функции
- `End` - Окончание функции
- `OriginNode` - Начальный узел
- `DirectionNode` - Узел направления системы координат
- `Type` - Тип функции
- `NumberOfPoints` - Количество точек (при постоянном шаге полилинии)
- `ClosedSpline` - Замкнутый сплайн
- `ConvertToSpline` - Создавать сплайн по полилинии
- `SplinePoints` - Количество точек сплайна
- `CurvatureOptimization` - Оптимизировать по кривизне
- `CurvatureTolerance` - Допуск при оптимизации по кривизне

### Унаследованные свойства от Construction:

- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым

## Заключение

Класс `FunctionConstruction` предоставляет мощные возможности для создания линий построения на основе математических функций в T-Flex CAD. Он поддерживает различные типы функций (обычные, параметрические), позволяет настраивать параметры отображения (количество точек, преобразование в сплайн), а также оптимизацию по кривизне. Функции могут быть интегрированы с другими объектами для создания сложных геометрических конструкций.
# FunctionConstruction - База знаний для RAG-системы

## Общее описание

FunctionConstruction представляет собой функциональную линию построения в T-Flex CAD API. Это геометрический элемент для создания кривых, определяемых математическими функциями.

## Основные характеристики

- Тип: Функциональная линия построения
- Назначение: Создание кривых на основе математических функций
- Использование: Создание сложных кривых форм, графиков функций, специализированных кривых
- Связь с другими объектами: Может использоваться как параметр для создания других геометрических объектов, источник для копирования

## Конструкторы

1. `FunctionConstruction(Document doc)` - Создает пустую функциональную линию построения

## Свойства

- `FunctionType` - Тип функции (FunctionType)
- `Parameter1` - Первый параметр функции (DoubleParameter)
- `Parameter2` - Второй параметр функции (DoubleParameter)
- `Parameter3` - Третий параметр функции (DoubleParameter)
- `StartParameter` - Начальное значение параметра (DoubleParameter)
- `EndParameter` - Конечное значение параметра (DoubleParameter)
- `GeometryType` - Тип геометрии линии построения
- `SubType` - Подтип линии построения
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

## Методы

- `SetFunction(FunctionType type, double param1, double param2, double param3)` - Установка типа функции и параметров
- `SetParameterRange(double start, double end)` - Установка диапазона параметров
- `GetPointAtParameter(double parameter)` - Получение точки на кривой по параметру
- `GetTangentAtParameter(double parameter)` - Получение касательной в точке кривой по параметру
- `GetLength()` - Получение длины кривой
- `IsPointOnCurve(Node point, double tolerance)` - Проверка, находится ли точка на кривой с заданной точностью

## Паттерны использования

1. Создание графиков математических функций
2. Определение специализированных кривых форм
3. Создание контуров сложных объектов
4. Использование в качестве базы для CopyConstruction
5. Создание вспомогательных элементов (кривые направляющие)

## Интеграция с другими объектами

- Может быть источником для CopyConstruction
- Может использоваться как база для SymmetryConstruction
- Может быть частью PathConstruction
- Может использоваться как ограничитель для других геометрических объектов
- Может быть источником для создания ConstructionNode и OutlineNode

## Примеры использования

### Базовое использование

```csharp
// Создание простой функциональной кривой (парабола)
FunctionConstruction parabola = new FunctionConstruction(document);
// В реальной реализации потребуется определение типа функции
// parabola.SetFunction(FunctionType.Parabola, 0.1, 0, 0);
// parabola.SetParameterRange(-20, 20);
parabola.Color = 255; // Красный цвет
```

### Создание синусоидальной кривой

```csharp
// Создание синусоидальной кривой
FunctionConstruction sineWave = new FunctionConstruction(document);
// В реальной реализации потребуется определение типа функции
// sineWave.SetFunction(FunctionType.Sine, 10, 1, 0);
// sineWave.SetParameterRange(0, 4 * Math.PI);
sineWave.Color = 65280; // Зеленый цвет
```

## Продвинутое использование

### Создание сложных функциональных кривых

```csharp
// Создание сложной функциональной кривой
FunctionConstruction complexCurve = new FunctionConstruction(document);

// В реальной реализации потребуется определение сложной функции
// Например, комбинация синуса и косинуса
// complexCurve.SetFunction(FunctionType.Custom, 0, 0, 0);
// complexCurve.SetParameterRange(0, 4 * Math.PI);

// Установка параметров для сложной функции
// complexCurve.Parameter1.Value = 5; // Амплитуда
// complexCurve.Parameter2.Value = 2; // Частота
// complexCurve.Parameter3.Value = 0.5; // Фаза

complexCurve.Color = 16711680; // Синий цвет
complexCurve.LineWidth = 2;
```

### Создание параметризованной системы функциональных кривых

```csharp
// Создание параметризованной системы функциональных кривых
int curveCount = 5;
FunctionConstruction[] parametricCurves = new FunctionConstruction[curveCount];

for (int i = 0; i < curveCount; i++)
{
    parametricCurves[i] = new FunctionConstruction(document);
    
    // В реальной реализации потребуется определение типа функции
    // parametricCurves[i].SetFunction(FunctionType.Sine, 5 + i * 2, 1 + i * 0.2, i * Math.PI / 4);
    // parametricCurves[i].SetParameterRange(0, 4 * Math.PI);
    
    // Установка цвета
    int red = (int)(255 * (double)i / (curveCount - 1));
    int green = 255 - red;
    int blue = 128;
    parametricCurves[i].Color = (red << 16) | (green << 8) | blue;
    parametricCurves[i].Style = LineStyle.Dash;
}
```

### Интеграция с другими объектами

```csharp
// Создание функциональной кривой, интегрированной с другими объектами
FunctionConstruction mainCurve = new FunctionConstruction(document);

// В реальной реализации потребуется определение функции
// mainCurve.SetFunction(FunctionType.Sine, 10, 1, 0);
// mainCurve.SetParameterRange(0, 4 * Math.PI);

mainCurve.Color = 255; // Красный цвет

// Создание точек на кривой
int pointOnCurveCount = 8;
FreeNode[] pointsOnCurve = new FreeNode[pointOnCurveCount];
double[] parameters = new double[pointOnCurveCount];

// Вычисление параметров для равномерного распределения точек
for (int i = 0; i < pointOnCurveCount; i++)
{
    // В реальной реализации потребуется метод получения точки на кривой по параметру
    // parameters[i] = mainCurve.StartParameter.Value + 
    //     (mainCurve.EndParameter.Value - mainCurve.StartParameter.Value) * i / (pointOnCurveCount - 1);
    // pointsOnCurve[i] = mainCurve.GetPointAtParameter(parameters[i]);
    
    // Для примера создаем приблизительные точки
    double t = 4 * Math.PI * i / (pointOnCurveCount - 1);
    double x = 20 + t * 10;
    double y = 50 + 10 * Math.Sin(t);
    pointsOnCurve[i] = new FreeNode(document, x, y);
    
    // Создание визуальных маркеров точек
    CircleConstruction marker = new CircleConstruction(document);
    marker.SetCenterAndRadius(pointsOnCurve[i], 1.5);
    marker.Color = 16776960; // Желтый цвет
}
```

### Оптимизация производительности

```csharp
// Создание большого количества функциональных кривых с оптимизацией
int curveCount = 30;
FunctionConstruction[] curves = new FunctionConstruction[curveCount];

// Создание кривых с различными параметрами
for (int i = 0; i < curveCount; i++)
{
    curves[i] = new FunctionConstruction(document);
    
    // В реальной реализации потребуется определение функции
    // curves[i].SetFunction(FunctionType.Sine, 2 + (i % 5), 0.5 + (i % 3) * 0.2, i * Math.PI / 15);
    // curves[i].SetParameterRange(0, 4 * Math.PI);
    
    // Установка цвета
    curves[i].Color = (i * 30) % 256;
}
```

### Работа с динамическими функциональными кривыми

```csharp
// Создание динамической функциональной кривой
FunctionConstruction dynamicCurve = new FunctionConstruction(document);

// В реальной реализации потребуется определение функции
// dynamicCurve.SetFunction(FunctionType.Sine, 10, 1, 0);
// dynamicCurve.SetParameterRange(0, 4 * Math.PI);

dynamicCurve.Color = 16711680; // Синий цвет

// В реальном приложении здесь могла бы быть логика обновления свойств кривой
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicCurve(double time)
{
    // Обновление параметров функции
    // dynamicCurve.Parameter1.Value = 10 + 5 * Math.Sin(time * 0.5); // Амплитуда
    // dynamicCurve.Parameter2.Value = 1 + 0.5 * Math.Cos(time * 0.3); // Частота
    // dynamicCurve.Parameter3.Value = time; // Фаза
    
    // Обновление цвета
    int red = (int)(255 * (1 + Math.Sin(time)) / 2);
    int green = (int)(255 * (1 + Math.Cos(time + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(time + 2 * Math.PI / 3)) / 2);
    dynamicCurve.Color = (red << 16) | (green << 8) | blue;
}
*/
```

## Связанные концепции

- SymmetryConstruction - Симметричная функциональная линия построения
- CopyConstruction - Копия функциональной линии построения
- OffsetConstruction - Смещенная функциональная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки и лучшие практики

1. Не забывайте использовать BeginChanges/EndChanges при создании множества функциональных кривых
2. Используйте параметризованные кривые для создания динамических конструкций
3. При создании больших массивов кривых используйте оптимизацию производительности
4. Убедитесь, что параметры функций находятся в допустимом диапазоне
5. Используйте кривые повторно при создании сложных конструкций
6. Проверяйте геометрические свойства кривых перед использованием в сложных расчетах

## Математические аспекты

- Функциональные кривые определяются математическими выражениями
- Точки на кривой вычисляются параметрически
- Касательные к кривой вычисляются через производные функций
- Длина кривой вычисляется численными методами
- Проверка принадлежности точки кривой осуществляется с заданной точностью

## Совместимость и ограничения

- FunctionConstruction совместим со всеми геометрическими объектами T-Flex CAD API
- Может использоваться как в 2D, так и в 3D построениях
- Ограничения связаны с сложностью определяющих функций
- При использовании в больших конструкциях может потребоваться оптимизация производительности

## Расширяемость

- FunctionConstruction может быть расширен через наследование для создания специализированных типов функциональных кривых
- Может быть интегрирован с пользовательскими математическими функциями
- Поддерживает пользовательские свойства через механизм параметров T-Flex
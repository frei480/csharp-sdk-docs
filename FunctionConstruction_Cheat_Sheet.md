# FunctionConstruction - Шпаргалка по классу в T-Flex CAD API

## Описание
FunctionConstruction представляет собой функциональную линию построения в T-Flex CAD API. Это геометрический элемент для создания кривых, определяемых математическими функциями.

## Основные свойства
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

## Конструкторы
```csharp
// Создание пустой функциональной линии построения
FunctionConstruction function = new FunctionConstruction(document);
```

## Основные методы
- `SetFunction(FunctionType type, double param1, double param2, double param3)` - Установка типа функции и параметров
- `SetParameterRange(double start, double end)` - Установка диапазона параметров
- `GetPointAtParameter(double parameter)` - Получение точки на кривой по параметру
- `GetTangentAtParameter(double parameter)` - Получение касательной в точке кривой по параметру
- `GetLength()` - Получение длины кривой
- `IsPointOnCurve(Node point, double tolerance)` - Проверка, находится ли точка на кривой с заданной точностью

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

## Связанные объекты
- SymmetryConstruction - Симметричная функциональная линия построения
- CopyConstruction - Копия функциональной линии построения
- OffsetConstruction - Смещенная функциональная линия построения
- PathConstruction - Путь построения
- FreeNode - Узел с абсолютными координатами
- ConstructionNode - Узел на линии построения
- OutlineNode - Узел на линии контура

## Частые ошибки
1. Не забывайте использовать BeginChanges/EndChanges при создании множества функциональных кривых
2. Убедитесь, что параметры функций находятся в допустимом диапазоне
3. Проверяйте геометрические свойства кривых перед использованием в сложных расчетах

## Лучшие практики
1. Используйте параметризованные кривые для создания динамических конструкций
2. При создании больших массивов кривых используйте оптимизацию производительности
3. Используйте кривые повторно при создании сложных конструкций
# FunctionConstruction - продвинутые примеры использования

Класс `FunctionConstruction` представляет линию построения-функцию в T-Flex CAD API. Этот класс предоставляет возможности для создания кривых на основе математических функций.

## Продвинутые примеры использования

### 1. Создание сложных математических функций

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание сложных математических функций");

// Создание функции в форме лемнискаты Бернулли
FunctionConstruction lemniscate = new FunctionConstruction(document);
lemniscate.FunctionName = "Лемниската Бернулли";

// Параметрическое представление лемнискаты
// x = a * cos(t) / (1 + sin^2(t))
// y = a * sin(t) * cos(t) / (1 + sin^2(t))
lemniscate.FirstTerm = "20 * cos(#1) / (1 + sin(#1)**2)"; // x-координата
lemniscate.SecondTerm = "20 * sin(#1) * cos(#1) / (1 + sin(#1)**2)"; // y-координата
lemniscate.Start = 0;
lemniscate.End = 2 * Math.PI;
lemniscate.Type = FunctionConstruction.FunctionType.Parametric;

// Установка системы координат
FreeNode lemniscateOrigin = new FreeNode(document, 50, 50);
FreeNode lemniscateDirection = new FreeNode(document, 55, 50);
lemniscate.OriginNode = lemniscateOrigin;
lemniscate.DirectionNode = lemniscateDirection;
lemniscate.Color = 255; // Красный цвет

// Создание функции в форме спирали Архимеда
FunctionConstruction archimedesSpiral = new FunctionConstruction(document);
archimedesSpiral.FunctionName = "Спираль Архимеда";

// Параметрическое представление спирали Архимеда
// x = a * t * cos(t)
// y = a * t * sin(t)
archimedesSpiral.FirstTerm = "5 * #1 * cos(#1)"; // x-координата
archimedesSpiral.SecondTerm = "5 * #1 * sin(#1)"; // y-координата
archimedesSpiral.Start = 0;
archimedesSpiral.End = 6 * Math.PI;
archimedesSpiral.Type = FunctionConstruction.FunctionType.Parametric;

// Установка системы координат
FreeNode spiralOrigin = new FreeNode(document, 120, 50);
FreeNode spiralDirection = new FreeNode(document, 125, 50);
archimedesSpiral.OriginNode = spiralOrigin;
archimedesSpiral.DirectionNode = spiralDirection;
archimedesSpiral.Color = 65280; // Зеленый цвет

// Создание функции в форме кардиоиды
FunctionConstruction cardioid = new FunctionConstruction(document);
cardioid.FunctionName = "Кардиоида";

// Параметрическое представление кардиоиды
// x = 2 * a * cos(t) * (1 + cos(t))
// y = 2 * a * sin(t) * (1 + cos(t))
cardioid.FirstTerm = "15 * cos(#1) * (1 + cos(#1))"; // x-координата
cardioid.SecondTerm = "15 * sin(#1) * (1 + cos(#1))"; // y-координата
cardioid.Start = 0;
cardioid.End = 2 * Math.PI;
cardioid.Type = FunctionConstruction.FunctionType.Parametric;

// Установка системы координат
FreeNode cardioidOrigin = new FreeNode(document, 50, 120);
FreeNode cardioidDirection = new FreeNode(document, 55, 120);
cardioid.OriginNode = cardioidOrigin;
cardioid.DirectionNode = cardioidDirection;
cardioid.Color = 16711680; // Синий цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 2. Создание функций с геометрическими преобразованиями

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание функций с геометрическими преобразованиями");

// Создание исходной функции (параболы)
FunctionConstruction sourceParabola = new FunctionConstruction(document);
sourceParabola.FunctionName = "Парабола";
sourceParabola.FirstTerm = "0.1 * #1**2"; // y = 0.1 * x^2
sourceParabola.Start = -30;
sourceParabola.End = 30;
sourceParabola.Type = FunctionConstruction.FunctionType.Plain;

// Установка системы координат
FreeNode parabolaOrigin = new FreeNode(document, 50, 50);
FreeNode parabolaDirection = new FreeNode(document, 55, 50);
sourceParabola.OriginNode = parabolaOrigin;
sourceParabola.DirectionNode = parabolaDirection;
sourceParabola.Color = 255; // Красный цвет

// Создание преобразованных функций
int transformCount = 6;
FunctionConstruction[] transformedFunctions = new FunctionConstruction[transformCount];

for (int i = 0; i < transformCount; i++)
{
    transformedFunctions[i] = new FunctionConstruction(document);
    transformedFunctions[i].FunctionName = "Преобразованная парабола " + (i + 1);
    
    // Различные преобразования
    switch (i)
    {
        case 0: // Смещение по вертикали
            transformedFunctions[i].FirstTerm = "0.1 * #1**2 + 10";
            break;
        case 1: // Смещение по горизонтали
            transformedFunctions[i].FirstTerm = "0.1 * (#1 - 5)**2";
            break;
        case 2: // Изменение масштаба
            transformedFunctions[i].FirstTerm = "0.2 * #1**2";
            break;
        case 3: // Отражение
            transformedFunctions[i].FirstTerm = "-0.1 * #1**2";
            break;
        case 4: // Комбинация преобразований
            transformedFunctions[i].FirstTerm = "0.1 * (#1 - 10)**2 + 15";
            break;
        case 5: // Кубическая функция
            transformedFunctions[i].FirstTerm = "0.01 * #1**3";
            transformedFunctions[i].Start = -20;
            transformedFunctions[i].End = 20;
            break;
    }
    
    transformedFunctions[i].Start = sourceParabola.Start;
    transformedFunctions[i].End = sourceParabola.End;
    transformedFunctions[i].Type = FunctionConstruction.FunctionType.Plain;
    
    // Установка системы координат с небольшим смещением
    FreeNode origin = new FreeNode(document, 50 + i * 5, 50 + i * 3);
    FreeNode direction = new FreeNode(document, 55 + i * 5, 50 + i * 3);
    transformedFunctions[i].OriginNode = origin;
    transformedFunctions[i].DirectionNode = direction;
    
    // Установка цвета
    int red = (int)(255 * (1 + Math.Sin(2 * Math.PI * i / transformCount)) / 2);
    int green = (int)(255 * (1 + Math.Cos(2 * Math.PI * i / transformCount + Math.PI / 3)) / 2);
    int blue = (int)(255 * (1 + Math.Sin(2 * Math.PI * i / transformCount + 2 * Math.PI / 3)) / 2);
    transformedFunctions[i].Color = (red << 16) | (green << 8) | blue;
}

// Создание функции с масштабированием по осям
FunctionConstruction scaledFunction = new FunctionConstruction(document);
scaledFunction.FunctionName = "Масштабированная функция";
scaledFunction.FirstTerm = "0.05 * #1**2"; // y = 0.05 * x^2
scaledFunction.Start = -40;
scaledFunction.End = 40;
scaledFunction.Type = FunctionConstruction.FunctionType.Plain;

// Установка системы координат с масштабированием
FreeNode scaledOrigin = new FreeNode(document, 50, 150);
FreeNode scaledDirection = new FreeNode(document, 52, 150); // Масштабирование по X
scaledFunction.OriginNode = scaledOrigin;
scaledFunction.DirectionNode = scaledDirection;
scaledFunction.Color = 16776960; // Желтый цвет

// Закрытие блока изменений документа
document.EndChanges();
```

### 3. Создание функций с использованием массивов и параметризации

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Создание параметризованной системы функций");

// Создание параметризованной системы синусоид
int sineCount = 5;
FunctionConstruction[] sineFunctions = new FunctionConstruction[sineCount];

for (int i = 0; i < sineCount; i++)
{
    sineFunctions[i] = new FunctionConstruction(document);
    sineFunctions[i].FunctionName = "Синусоида " + (i + 1);
    
    // Параметрическая амплитуда и частота
    double amplitude = 5 + i * 3;
    double frequency = 0.2 + i * 0.1;
    sineFunctions[i].FirstTerm = amplitude + " * sin(" + frequency + " * #1)";
    
    sineFunctions[i].Start = 0;
    sineFunctions[i].End = 4 * Math.PI;
    sineFunctions[i].Type = FunctionConstruction.FunctionType.Plain;
    
    // Установка системы координат
    FreeNode origin = new FreeNode(document, 30, 30 + i * 20);
    FreeNode direction = new FreeNode(document, 35, 30 + i * 20);
    sineFunctions[i].OriginNode = origin;
    sineFunctions[i].DirectionNode = direction;
    
    // Установка цвета с градиентом
    int red = (int)(255 * (double)i / (sineCount - 1));
    int green = (int)(255 * (1 - (double)i / (sineCount - 1)));
    int blue = 128;
    sineFunctions[i].Color = (red << 16) | (green << 8) | blue;
}

// Создание параметризованной системы экспоненциальных функций
int expCount = 4;
FunctionConstruction[] expFunctions = new FunctionConstruction[expCount];

for (int i = 0; i < expCount; i++)
{
    expFunctions[i] = new FunctionConstruction(document);
    expFunctions[i].FunctionName = "Экспонента " + (i + 1);
    
    // Параметрический коэффициент
    double coefficient = 0.1 + i * 0.05;
    expFunctions[i].FirstTerm = "exp(" + coefficient + " * #1)";
    
    expFunctions[i].Start = -5;
    expFunctions[i].End = 5;
    expFunctions[i].Type = FunctionConstruction.FunctionType.Plain;
    
    // Установка системы координат
    FreeNode origin = new FreeNode(document, 100, 30 + i * 30);
    FreeNode direction = new FreeNode(document, 105, 30 + i * 30);
    expFunctions[i].OriginNode = origin;
    expFunctions[i].DirectionNode = direction;
    
    // Установка цвета
    int red = 255;
    int green = (int)(255 * (1 - (double)i / (expCount - 1)));
    int blue = (int)(255 * (double)i / (expCount - 1));
    expFunctions[i].Color = (red << 16) | (green << 8) | blue;
}

// Создание параметризованной системы полиномиальных функций
int polyCount = 3;
FunctionConstruction[] polyFunctions = new FunctionConstruction[polyCount];

for (int i = 0; i < polyCount; i++)
{
    polyFunctions[i] = new FunctionConstruction(document);
    polyFunctions[i].FunctionName = "Полином " + (i + 1);
    
    // Параметрический полином
    switch (i)
    {
        case 0:
            polyFunctions[i].FirstTerm = "0.01 * #1**3 - 0.2 * #1";
            break;
        case 1:
            polyFunctions[i].FirstTerm = "0.001 * #1**4 - 0.05 * #1**2 + 2";
            break;
        case 2:
            polyFunctions[i].FirstTerm = "0.0001 * #1**5 - 0.01 * #1**3 + 0.5 * #1";
            break;
    }
    
    polyFunctions[i].Start = -20;
    polyFunctions[i].End = 20;
    polyFunctions[i].Type = FunctionConstruction.FunctionType.Plain;
    
    // Установка системы координат
    FreeNode origin = new FreeNode(document, 30, 150 + i * 40);
    FreeNode direction = new FreeNode(document, 35, 150 + i * 40);
    polyFunctions[i].OriginNode = origin;
    polyFunctions[i].DirectionNode = direction;
    
    // Установка цвета
    int red = (int)(255 * (double)i / (polyCount - 1));
    int green = 128;
    int blue = (int)(255 * (1 - (double)i / (polyCount - 1)));
    polyFunctions[i].Color = (red << 16) | (green << 8) | blue;
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 4. Интеграция функций с другими объектами

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Интеграция функций с другими объектами");

// Создание функции и связанных объектов
FunctionConstruction mainFunction = new FunctionConstruction(document);
mainFunction.FunctionName = "Главная функция";
mainFunction.FirstTerm = "10 * sin(0.5 * #1)"; // y = 10 * sin(0.5 * x)
mainFunction.Start = 0;
mainFunction.End = 4 * Math.PI;
mainFunction.Type = FunctionConstruction.FunctionType.Plain;

// Установка системы координат
FreeNode functionOrigin = new FreeNode(document, 50, 50);
FreeNode functionDirection = new FreeNode(document, 55, 50);
mainFunction.OriginNode = functionOrigin;
mainFunction.DirectionNode = functionDirection;
mainFunction.Color = 255; // Красный цвет

// Создание точек на функции
int pointCount = 12;
FreeNode[] functionPoints = new FreeNode[pointCount];
CircleConstruction[] pointMarkers = new CircleConstruction[pointCount];

for (int i = 0; i < pointCount; i++)
{
    double t = mainFunction.Start + (mainFunction.End - mainFunction.Start) * i / (pointCount - 1);
    double x = functionOrigin.X.Value + (t - mainFunction.Start) * 5; // Масштабирование
    double y = functionOrigin.Y.Value + 10 * Math.Sin(0.5 * t);
    functionPoints[i] = new FreeNode(document, x, y);
    
    // Создание визуальных маркеров точек
    pointMarkers[i] = new CircleConstruction(document);
    pointMarkers[i].SetCenterAndRadius(functionPoints[i], 1.5);
    pointMarkers[i].Color = 65280; // Зеленый цвет
}

// Создание касательных линий к функции
int tangentCount = 6;
LineConstruction[] tangentLines = new LineConstruction[tangentCount];

for (int i = 0; i < tangentCount; i++)
{
    int pointIndex = i * (pointCount - 1) / (tangentCount - 1);
    if (pointIndex >= pointCount) pointIndex = pointCount - 1;
    
    FreeNode point = functionPoints[pointIndex];
    
    // Вычисление направления касательной (приблизительно)
    double tangentLength = 15;
    double derivative = 5 * Math.Cos(0.5 * (mainFunction.Start + (mainFunction.End - mainFunction.Start) * pointIndex / (pointCount - 1)));
    double tangentAngle = Math.Atan(derivative);
    double endX = point.X.Value + tangentLength * Math.Cos(tangentAngle);
    double endY = point.Y.Value + tangentLength * Math.Sin(tangentAngle);
    
    FreeNode endPoint = new FreeNode(document, endX, endY);
    tangentLines[i] = new LineConstruction(document);
    tangentLines[i].SetTwoNodes(point, endPoint);
    tangentLines[i].Color = 16711680; // Синий цвет
}

// Создание нормалей к функции
int normalCount = 6;
LineConstruction[] normalLines = new LineConstruction[normalCount];

for (int i = 0; i < normalCount; i++)
{
    int pointIndex = i * (pointCount - 1) / (normalCount - 1);
    if (pointIndex >= pointCount) pointIndex = pointCount - 1;
    
    FreeNode point = functionPoints[pointIndex];
    
    // Вычисление направления нормали (перпендикулярно касательной)
    double normalLength = 12;
    double derivative = 5 * Math.Cos(0.5 * (mainFunction.Start + (mainFunction.End - mainFunction.Start) * pointIndex / (pointCount - 1)));
    double normalAngle = Math.Atan(derivative) + Math.PI / 2;
    double endX = point.X.Value + normalLength * Math.Cos(normalAngle);
    double endY = point.Y.Value + normalLength * Math.Sin(normalAngle);
    
    FreeNode endPoint = new FreeNode(document, endX, endY);
    normalLines[i] = new LineConstruction(document);
    normalLines[i].SetTwoNodes(point, endPoint);
    normalLines[i].Color = 16776960; // Желтый цвет
}

// Создание функции, интегрированной с контуром
PathConstruction integrationPath = new PathConstruction(document);

// Создание контура, представляющего площадь под кривой
FreeNode[] areaNodes = new FreeNode[pointCount + 2];
for (int i = 0; i < pointCount; i++)
{
    areaNodes[i] = functionPoints[i];
}
areaNodes[pointCount] = new FreeNode(document, functionPoints[pointCount - 1].X.Value, functionOrigin.Y.Value);
areaNodes[pointCount + 1] = new FreeNode(document, functionPoints[0].X.Value, functionOrigin.Y.Value);

for (int i = 0; i <= pointCount; i++)
{
    integrationPath.AddSegment(areaNodes[i], areaNodes[(i + 1) % (pointCount + 2)]);
}

integrationPath.Color = 16711935; // Пурпурный цвет
integrationPath.Style = LineStyle.Dash; // Пунктирная линия

// Закрытие блока изменений документа
document.EndChanges();
```

### 5. Оптимизация производительности при работе с множеством функций

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Оптимизация производительности");

// Создание большого количества функций с минимальными вызовами API
int functionCount = 50;
FunctionConstruction[] functions = new FunctionConstruction[functionCount];

// Предварительное создание узлов
FreeNode[,] originNodes = new FreeNode[functionCount, 2];

Random random = new Random();
for (int i = 0; i < functionCount; i++)
{
    originNodes[i, 0] = new FreeNode(document, 
        20 + random.NextDouble() * 160, 
        20 + random.NextDouble() * 110);
    originNodes[i, 1] = new FreeNode(document, 
        originNodes[i, 0].X.Value + 5, 
        originNodes[i, 0].Y.Value);
}

// Создание функций
for (int i = 0; i < functionCount; i++)
{
    functions[i] = new FunctionConstruction(document);
    functions[i].FunctionName = "Функция " + (i + 1);
    
    // Случайная функция
    int functionType = random.Next(4);
    switch (functionType)
    {
        case 0: // Линейная
            functions[i].FirstTerm = (random.NextDouble() * 2 - 1) + " * #1 + " + (random.NextDouble() * 20 - 10);
            functions[i].Start = -10;
            functions[i].End = 10;
            break;
        case 1: // Квадратичная
            functions[i].FirstTerm = (random.NextDouble() * 0.1 - 0.05) + " * #1**2 + " + (random.NextDouble() * 2 - 1) + " * #1 + " + (random.NextDouble() * 10 - 5);
            functions[i].Start = -15;
            functions[i].End = 15;
            break;
        case 2: // Синусоидальная
            functions[i].FirstTerm = (random.NextDouble() * 5 + 1) + " * sin(" + (random.NextDouble() * 0.5 + 0.1) + " * #1 + " + (random.NextDouble() * Math.PI) + ")";
            functions[i].Start = 0;
            functions[i].End = 4 * Math.PI;
            break;
        case 3: // Экспоненциальная
            functions[i].FirstTerm = (random.NextDouble() * 0.2 + 0.05) + " * exp(" + (random.NextDouble() * 0.1 + 0.02) + " * #1)";
            functions[i].Start = -5;
            functions[i].End = 5;
            break;
    }
    
    functions[i].Type = FunctionConstruction.FunctionType.Plain;
    functions[i].OriginNode = originNodes[i, 0];
    functions[i].DirectionNode = originNodes[i, 1];
    
    // Установка цвета
    int red = (int)(255 * random.NextDouble());
    int green = (int)(255 * random.NextDouble());
    int blue = (int)(255 * random.NextDouble());
    functions[i].Color = (red << 16) | (green << 8) | blue;
    
    // Установка толщины линии
    functions[i].LineWidth = 1 + (int)(random.NextDouble() * 2);
}

// Закрытие блока изменений документа
document.EndChanges();
```

### 6. Работа с динамическими функциями и обновление свойств

```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Открытие блока изменений документа
document.BeginChanges("Динамические функции");

// Создание функции с возможностью динамического обновления
FunctionConstruction dynamicFunction = new FunctionConstruction(document);
dynamicFunction.FunctionName = "Динамическая функция";
dynamicFunction.FirstTerm = "10 * sin(0.5 * #1)"; // y = 10 * sin(0.5 * x)
dynamicFunction.Start = 0;
dynamicFunction.End = 4 * Math.PI;
dynamicFunction.Type = FunctionConstruction.FunctionType.Plain;

// Установка системы координат
FreeNode dynamicOrigin = new FreeNode(document, 50, 50);
FreeNode dynamicDirection = new FreeNode(document, 55, 50);
dynamicFunction.OriginNode = dynamicOrigin;
dynamicFunction.DirectionNode = dynamicDirection;
dynamicFunction.Color = 255; // Красный цвет

// Создание функции, которая будет менять свои параметры
FunctionConstruction morphingFunction = new FunctionConstruction(document);
morphingFunction.FunctionName = "Морфирующая функция";
morphingFunction.FirstTerm = "5 * sin(#1)"; // y = 5 * sin(x)
morphingFunction.Start = 0;
morphingFunction.End = 2 * Math.PI;
morphingFunction.Type = FunctionConstruction.FunctionType.Plain;

// Установка системы координат
FreeNode morphingOrigin = new FreeNode(document, 120, 50);
FreeNode morphingDirection = new FreeNode(document, 125, 50);
morphingFunction.OriginNode = morphingOrigin;
morphingFunction.DirectionNode = morphingDirection;
morphingFunction.Color = 65280; // Зеленый цвет

// Создание системы функций с анимацией
int animatedFunctionCount = 6;
FunctionConstruction[] animatedFunctions = new FunctionConstruction[animatedFunctionCount];

for (int i = 0; i < animatedFunctionCount; i++)
{
    animatedFunctions[i] = new FunctionConstruction(document);
    animatedFunctions[i].FunctionName = "Анимированная функция " + (i + 1);
    animatedFunctions[i].FirstTerm = "sin(#1 + " + (i * Math.PI / 3) + ")"; // y = sin(x + phase)
    animatedFunctions[i].Start = 0;
    animatedFunctions[i].End = 2 * Math.PI;
    animatedFunctions[i].Type = FunctionConstruction.FunctionType.Plain;
    
    // Установка системы координат
    FreeNode origin = new FreeNode(document, 50 + i * 25, 100);
    FreeNode direction = new FreeNode(document, 55 + i * 25, 100);
    animatedFunctions[i].OriginNode = origin;
    animatedFunctions[i].DirectionNode = direction;
    animatedFunctions[i].Color = 16711680; // Синий цвет
}

// Закрытие блока изменений документа
document.EndChanges();

// В реальном приложении здесь могла бы быть логика обновления свойств функций
// Например, в обработчике таймера или событий:
/*
public void UpdateDynamicFunctions(double time)
{
    // Открытие блока изменений документа
    document.BeginChanges("Обновление динамических функций");
    
    // Обновление параметров динамической функции
    double newAmplitude = 10 + 5 * Math.Sin(time * 0.5);
    double newFrequency = 0.5 + 0.2 * Math.Cos(time * 0.3);
    dynamicFunction.FirstTerm = newAmplitude + " * sin(" + newFrequency + " * #1)";
    
    // Обновление параметров морфирующей функции
    double morphingAmplitude = 5 + 3 * Math.Sin(time * 0.7);
    double morphingFrequency = 1 + 0.5 * Math.Cos(time * 0.4);
    morphingFunction.FirstTerm = morphingAmplitude + " * sin(" + morphingFrequency + " * #1)";
    
    // Обновление анимированных функций
    for (int i = 0; i < animatedFunctionCount; i++)
    {
        double phase = i * Math.PI / 3 + time * 0.5;
        animatedFunctions[i].FirstTerm = "sin(#1 + " + phase + ")";
        
        // Изменение цвета в зависимости от времени
        int red = (int)(255 * (1 + Math.Sin(time * 0.3 + i)) / 2);
        int green = (int)(255 * (1 + Math.Cos(time * 0.3 + i + 1)) / 2);
        int blue = (int)(255 * (1 + Math.Sin(time * 0.3 + i + 2)) / 2);
        animatedFunctions[i].Color = (red << 16) | (green << 8) | blue;
    }
    
    // Закрытие блока изменений документа
    document.EndChanges();
}
*/
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
- `Color` - Цвет объекта
- `Layer` - Слой, на котором размещается объект
- `Level` - Уровень объекта
- `Visible` - Является ли объект видимым
- `LineWidth` - Толщина линии
- `Style` - Стиль линии

### Основные методы:

- `SetFunction` - Установка функции
- `SetRange` - Установка диапазона
- `SetOriginNode` - Установка начального узла
- `SetDirectionNode` - Установка узла направления
- `SetFunctionType` - Установка типа функции
- `GetFunctionGeometry` - Получение геометрии функции

## Заключение

Продвинутое использование класса `FunctionConstruction` включает в себя создание сложных математических функций, применение геометрических преобразований, параметризованные конструкции, интеграцию с другими объектами, оптимизацию производительности и реализацию динамических конструкций. При работе с большими наборами функций важно учитывать производительность и использовать эффективные алгоритмы для вычисления значений функций и установления связей между объектами.
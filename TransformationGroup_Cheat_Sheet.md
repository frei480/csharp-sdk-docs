# Шпаргалка по классу TransformationGroup в T-Flex CAD API

## Основные классы

- **TransformationGroup** - Группа трансформаций (наследник TransformationGroupBase)
- **TransformationGroupBase** - Базовый класс групп трансформаций
- **TransformationGroupContainer** - Контейнер групп трансформаций

## Создание трансформаций

```csharp
// Получение контейнера трансформаций объекта
TransformationGroupContainer container = object3D.Transformations;

// Создание новой группы трансформаций
TransformationGroup group = container.AddBaseTransfGroup();
group.Name = "Новая группа";
```

## Основные методы TransformationGroup

### Перемещения
```csharp
// Перемещение по оси
group.AddMoveTransf(TransformationCoordinate.X, offsetParam);

// Перемещение до точки (все оси)
group.AddMoveToNodeTransf(targetPoint);

// Перемещение по оси до точки
group.AddMoveToNodeTransf(TransformationCoordinate.X, targetPoint);

// Перемещение до поверхности
group.AddMoveToSurfaceTransf(TransformationCoordinate.Z, surface);

// Перемещение до кривой
group.AddMoveToCurveTransf(TransformationCoordinate.X, curve);
```

### Вращения
```csharp
// Вращение вокруг оси
group.AddRotateTransf(TransformationCoordinate.Z, angleParam);
```

### Ориентация осей
```csharp
// Совмещение оси с другой осью
group.AddSetAxisTransf(TransformationCoordinate.X, targetAxis);

// Совмещение оси с направлением
group.AddSetAxisDirectionTransf(TransformationCoordinate.X, direction);

// Направление оси на точку
group.AddDirectAxisToPointTransf(TransformationCoordinate.Z, targetPoint);

// Поворот оси вокруг другой оси к точке
group.AddDirectAxisByAxisToPointTransf(
    TransformationCoordinate.X,  // неподвижная ось
    TransformationCoordinate.Y,  // поворачиваемая ось
    targetPoint);

// Поворот оси вокруг другой оси по направлению
group.AddDirectAxisByAxisToDirectionTransf(
    TransformationCoordinate.X,  // неподвижная ось
    TransformationCoordinate.Y,  // поворачиваемая ось
    direction);
```

### Матричные трансформации
```csharp
// Применение аффинной трансформации
group.AddMap(affineTransform);
```

### Работа с ЛСК
```csharp
// Получение ЛСК
LCS currentLCS = group.GetLCS();

// Установка ЛСК
group.SetLCS(newLCS, true); // true - пересчитать координаты
```

## Свойства TransformationGroup

- `IndexInContainer` - Индекс в контейнере
- `IsValid` - Актуальность группы
- `Name` - Имя группы
- `Suppressed` - Подавление группы (>0 подавлена)
- `TransfContainer` - Родительский контейнер

## Работа с контейнером

### Создание и получение групп
```csharp
// Создание новой группы
TransformationGroup newGroup = container.AddBaseTransfGroup();

// Получение количества групп
int count = container.GetBaseTransfCount();

// Получение всех групп
List<TransformationGroup> groups = container.GetBaseTransfGroups();

// Получение группы по индексу
TransformationGroup group = container.GetBaseTransfGroupAt(0);
```

### Управление группами
```csharp
// Удаление группы по индексу
container.DeleteBaseTransfGroup(1);

// Удаление всех групп
container.DeleteAllBaseTransfGroups();

// Перемещение группы вверх
TransformationGroup movedUp = container.MoveBaseTransfGroupUp(group);

// Перемещение группы вниз
TransformationGroup movedDown = container.MoveBaseTransfGroupDown(group);
```

### Преобразование трансформаций
```csharp
// Преобразование в неассоциативную трансформацию
bool success = container.MakeNonAssociative();
```

## Свойства контейнера

- `Owner` - Владелец контейнера (Object3D)
- `SourceCSType` - Тип исходной системы координат

## Перечисления

### TransformationCoordinate
- `X` - Ось X
- `Y` - Ось Y
- `Z` - Ось Z

## Полезные советы

1. **Именуйте группы** - Используйте осмысленные имена для групп трансформаций
2. **Порядок важен** - Трансформации применяются в порядке добавления групп
3. **Параметризация** - Используйте Parameter для гибкого управления
4. **Подавление** - Используйте свойство Suppressed для условного применения
5. **Проверка актуальности** - Всегда проверяйте свойство IsValid перед использованием

## Частые ошибки

1. **Использование устаревших групп** - Всегда проверяйте IsValid после перемещения групп
2. **Неправильный порядок трансформаций** - Помните, что порядок добавления важен
3. **Игнорирование подавления** - Не забывайте про свойство Suppressed
4. **Неправильная работа с ЛСК** - Учитывайте пересчет координат при изменении ЛСК

Эта шпаргалка охватывает основные аспекты работы с классом TransformationGroup в T-Flex CAD API.
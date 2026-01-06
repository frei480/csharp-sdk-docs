# Примеры использования класса TransformationGroup в T-Flex CAD API

## Основные сущности

### TransformationGroup
Группа трансформаций, наследуется от TransformationGroupBase.

### TransformationGroupBase
Базовый класс групп трансформаций.

### TransformationGroupContainer
Контейнер групп трансформаций.

## Базовые примеры использования

### 1. Создание новой группы трансформаций

```csharp
// Получаем контейнер трансформаций объекта
TransformationGroupContainer transfContainer = someObject3D.Transformations;

// Добавляем новую группу трансформаций
TransformationGroup transfGroup = transfContainer.AddBaseTransfGroup();

// Устанавливаем имя группы
transfGroup.Name = "Моя группа трансформаций";
```

### 2. Добавление простого перемещения

```csharp
// Создаем параметр для задания величины перемещения
Parameter offset = new Parameter(10.0); // 10 мм

// Добавляем перемещение по оси X
transfGroup.AddMoveTransf(TransformationCoordinate.X, offset);
```

### 3. Добавление вращения

```csharp
// Создаем параметр для задания угла поворота
Parameter angle = new Parameter(45.0); // 45 градусов

// Добавляем вращение вокруг оси Z
transfGroup.AddRotateTransf(TransformationCoordinate.Z, angle);
```

### 4. Перемещение до точки

```csharp
// Создаем точку назначения
ModelPoint3D targetPoint = new ModelPoint3D(50.0, 30.0, 0.0);

// Добавляем перемещение всех осей до заданной точки
transfGroup.AddMoveToNodeTransf(targetPoint);
```

### 5. Совмещение оси с направлением

```csharp
// Создаем направление
ModelDirection targetDirection = new ModelDirection(1.0, 0.0, 1.0);

// Совмещаем ось X с заданным направлением
transfGroup.AddSetAxisDirectionTransf(TransformationCoordinate.X, targetDirection);
```

### 6. Направление оси на точку

```csharp
// Создаем точку, на которую нужно направить ось
ModelPoint3D targetPoint = new ModelPoint3D(100.0, 50.0, 0.0);

// Направляем ось Z на заданную точку
transfGroup.AddDirectAxisToPointTransf(TransformationCoordinate.Z, targetPoint);
```

### 7. Получение и установка ЛСК группы

```csharp
// Получаем текущую ЛСК группы
LCS currentLCS = transfGroup.GetLCS();

// Создаем новую ЛСК
LCS newLCS = new LCS();
// ... настройка новой ЛСК ...

// Устанавливаем новую ЛСК для группы
transfGroup.SetLCS(newLCS, true); // true - пересчитать координаты
```

### 8. Работа с контейнером трансформаций

```csharp
// Получаем количество групп трансформаций
int groupCount = transfContainer.GetBaseTransfCount();

// Получаем список всех групп
List<TransformationGroup> groups = transfContainer.GetBaseTransfGroups();

// Получаем конкретную группу по индексу
TransformationGroup specificGroup = transfContainer.GetBaseTransfGroupAt(0);

// Удаляем группу по индексу
transfContainer.DeleteBaseTransfGroup(1);
```

### 9. Перемещение групп в контейнере

```csharp
// Получаем группу для перемещения
TransformationGroup groupToMove = transfContainer.GetBaseTransfGroupAt(0);

// Перемещаем группу вверх
TransformationGroup updatedGroup = transfContainer.MoveBaseTransfGroupUp(groupToMove);

// Перемещаем группу вниз
updatedGroup = transfContainer.MoveBaseTransfGroupDown(updatedGroup);
```

### 10. Преобразование в неассоциативную трансформацию

```csharp
// Преобразуем все трансформации в одну неассоциативную
bool success = transfContainer.MakeNonAssociative();
```

## Свойства классов

### TransformationGroup
- `IndexInContainer` - Индекс группы трансформации в контейнере
- `IsValid` - true, если группа трансформаций еще находится в контейнере
- `Name` - Имя группы
- `Suppressed` - Параметр подавления группы трансформаций
- `TransfContainer` - Контейнер групп трансформаций, которому принадлежит данная группа

### TransformationGroupContainer
- `Owner` - Объект, которому принадлежит контейнер
- `SourceCSType` - Тип исходной системы координат преобразования

Эти примеры демонстрируют основные возможности работы с трансформациями в T-Flex CAD API.
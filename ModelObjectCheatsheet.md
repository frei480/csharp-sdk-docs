# Шпаргалка по классу ModelObject в T-Flex CAD API

## Основные свойства

| Свойство | Описание |
|---------|----------|
| `ObjectId` | Уникальный ID объекта |
| `Name` | Имя объекта |
| `DisplayName` | Отображаемое имя |
| `Visible` | Видимость объекта |
| `Editable` | Режим редактирования |
| `Document` | Родительский документ |
| `X`, `Y` | Координаты объекта |

## Проверка типов

```csharp
// Проверка типа объекта
bool isText = modelObject.IsKindOf(ModelObjectType.Text);
bool isParagraph = modelObject.IsKindOf(ModelObjectType.ParagraphText);
bool isTable = modelObject.IsKindOf(ModelObjectType.Table);
```

## Работа с атрибутами

### Получение атрибутов
```csharp
// Получить атрибуты объекта
var attributes = modelObject.GetAttributes();

// Получить значения
int intValue = attributes.GetIntAttribute("имя");
string textValue = attributes.GetTextAttribute("имя");
double realValue = attributes.GetRealAttribute("имя");
```

### Установка атрибутов
```csharp
// Установить значения
attributes.SetIntAttribute("имя", значение, true);
attributes.SetTextAttribute("имя", "значение", true);
attributes.SetRealAttribute("имя", значение, true);
```

## Работа со свойствами

### Получение свойств
```csharp
// Вещественные свойства
double width = modelObject.GetRealProperty("Ширина");
double height = modelObject.GetRealProperty("Высота");

// Текстовые свойства
string description = modelObject.GetTextProperty("Описание");

// Целочисленные свойства
int count = modelObject.GetIntProperty("Количество");
```

## Работа с группами

### Создание группы
```csharp
// Создать группу
ModelObjectGroup group = new ModelObjectGroup(document);
group.Name = "Имя группы";

// Добавить объекты
group.Add(modelObject);
```

### Получение группы
```csharp
// Группа объекта
ModelObjectGroup group = modelObject.ModelObjectGroup;

// Объекты в группе
var groupObjects = group.Objects;
```

## Работа с родителями

### Получение родителей
```csharp
// Родительские объекты
var parents = modelObject.Parents;

// Количество родителей
int parentCount = parents.Count();
```

## Управление объектом

### Клонирование
```csharp
// Создать копию
ModelObject clone = modelObject.Clone();
```

### Удаление
```csharp
// Удалить объект
document.DeleteObjects(new List<ModelObject> { modelObject });
```

### Пересчет
```csharp
// Пересчитать объект
modelObject.Regenerate();
```

## Работа со связями

### Проверка зависимостей
```csharp
// Зависит ли объект от другого
bool depends = modelObject.DependsOn(otherObject);
```

### Получение связей
```csharp
// Получить ссылки
var references = modelObject.GetReferences();
```

## Полезные методы

| Метод | Описание |
|------|----------|
| `Clone()` | Создать копию объекта |
| `Regenerate()` | Пересчитать объект |
| `MarkChanged()` | Пометить как измененный |
| `CopyProperties()` | Копировать свойства |
| `PasteProperties()` | Вставить свойства |

## Частые ошибки

1. **Работа с удаленным объектом**
   - Проверяйте `IsDisposed` перед использованием

2. **Неправильная типизация**
   - Используйте `IsKindOf()` для проверки типа

3. **Проблемы с доступом**
   - Проверяйте `Editable` для редактируемых операций

## См. также
- [Document](DocumentCheatsheet.md)
- [ParagraphText](ParagraphTextCheatsheet.md)
- [Table](TableCheatsheet.md)
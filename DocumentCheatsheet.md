# Шпаргалка по классу Document в T-Flex CAD API

## Основные операции

### Получение документа
```csharp
// Активный документ
Document document = TFlex.Application.ActiveDocument;

// Проверка наличия документа
if (document != null)
{
    // Работа с документом
}
```

### Управление изменениями
```csharp
// Начало блока изменений
document.BeginChanges("Описание изменений");

// Применение изменений
document.ApplyChanges();

// Отмена изменений
document.CancelChanges();

// Завершение блока изменений
document.EndChanges();
```

### Сохранение документа
```csharp
// Сохранение
document.Save();

// Сохранение как
document.SaveAs("путь_к_файлу.имя_файла");

// Сохранение копии
document.SaveCopy("путь_к_файлу.имя_файла");
```

## Работа с объектами

### Получение объектов
```csharp
// Все объекты
var objects = document.GetObjects();

// Объект по ID
ModelObject obj = document.GetObjectById(id);

// Объект по имени
ModelObject obj = document.GetObjectByName("имя_объекта");
```

### Создание объектов
```csharp
// Текстовый блок
ParagraphText text = new ParagraphText(document);

// Многострочный текст
MultilineText multiline = new MultilineText(document);
```

## Работа с переменными

### Создание переменных
```csharp
// Вещественная переменная
Variable realVar = document.CreateRealVariable("имя", значение);

// Текстовая переменная
Variable textVar = document.CreateTextVariable("имя", "значение");
```

### Поиск переменных
```csharp
// Найти переменную
Variable var = document.FindVariable("имя_переменной");

// Все переменные
var variables = document.GetVariables();
```

## Работа со страницами

### Получение страниц
```csharp
// Все страницы
var pages = document.GetPages();

// Активная страница
Page activePage = document.ActivePage;
```

### Создание страниц
```csharp
// Новая страница
Page newPage = new Page(document, PageType.Normal);
```

## Работа с атрибутами

### Получение атрибутов
```csharp
// Атрибуты документа
var attributes = document.GetAttributes();

// Получение значений
int intValue = attributes.GetIntAttribute("имя");
string textValue = attributes.GetTextAttribute("имя");
double realValue = attributes.GetRealAttribute("имя");
```

### Установка атрибутов
```csharp
// Установка значений
attributes.SetIntAttribute("имя", значение, true);
attributes.SetTextAttribute("имя", "значение", true);
attributes.SetRealAttribute("имя", значение, true);
```

## Полезные свойства

| Свойство | Описание |
|---------|----------|
| `Title` | Имя документа |
| `FileName` | Полный путь к файлу |
| `Changed` | Признак изменений |
| `IsReadOnly` | Доступен ли для записи |
| `Visible` | Видимость документа |

## Частые ошибки

1. **Забытое BeginChanges()**
   - Всегда оборачивайте изменения в BeginChanges()/EndChanges()

2. **Работа с null документом**
   - Всегда проверяйте document != null

3. **Неправильное управление памятью**
   - Используйте using для временных объектов

## См. также
- [ModelObject](ModelObjectCheatsheet.md)
- [ParagraphText](ParagraphTextCheatsheet.md)
- [Table](TableCheatsheet.md)
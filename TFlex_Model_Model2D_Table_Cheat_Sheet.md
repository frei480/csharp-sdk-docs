# Шпаргалка по классу TFlex.Model.Model2D.Table в T-Flex CAD API

## Основная информация
- **Класс**: `Table`
- **Назначение**: Таблица в многострочном тексте
- **Пространство имен**: `TFlex.Model.Model2D`
- **Базовый класс**: `System.Object`

## Основные компоненты

### Table.CreationSettings
Настройки создания таблицы.

**Конструктор:**
```csharp
Table.CreationSettings(int columns, int rows)
```

**Свойства:**
- `ColumnsCount` (int) - Количество столбцов
- `RowsCount` (int) - Количество строк

### Table.CellProperties
Свойства ячеек таблицы.

**Свойства:**
- `CellWidth` (double) - Ширина ячейки
- `RowHeight` (double) - Высота строки
- `CellTextVAlign` (Table.TextVAlign) - Вертикальное выравнивание текста
- `CellTextHAlign` (Table.TextHAlign) - Горизонтальное выравнивание текста
- `TextDirection` (Table.TextDirection) - Направление текста
- `BackgroundColor` (int) - Цвет фона ячейки

### Table.InsertProperties
Позиция вставки строк/столбцов.

**Значения:**
- `Before` - Перед указанной ячейкой
- `After` - После указанной ячейки

## Основные методы

### Создание таблицы
```csharp
// Создание таблицы с настройками
Table.CreationSettings sett = new Table.CreationSettings(3, 2);
Table table = multilineText.CreateTable(sett);

// Создание таблицы с настройками и свойствами ячеек
Table.CellProperties prop = new Table.CellProperties();
Table table = multilineText.CreateTable(sett, prop);
```

### Работа с ячейками
```csharp
// Получение свойств ячейки
Table.CellProperties prop = table.GetCellProperties(0);

// Установка свойств ячейки
table.SetCellProperties(0, prop);

// Вставка текста в ячейку
table.InsertText(0, 0, "Текст");

// Вставка текста с форматом
CharFormat format = new CharFormat();
table.InsertText(0, 0, "Текст", format);

// Получение текста из ячейки
string text = table.GetCellText(0);

// Очистка ячейки
table.Clear(0);
```

### Управление структурой
```csharp
// Вставка строк
table.InsertRows(0, 2, Table.InsertProperties.After);

// Вставка столбцов
table.InsertColumns(0, 2, Table.InsertProperties.After);

// Удаление строки
table.DeleteRow(0);

// Удаление столбца
table.DeleteColumn(0);
```

### Работа с размерами
```csharp
// Получение ширины ячейки
double width = table.GetCellWidth(0);

// Установка ширины ячейки
table.SetCellWidth(0, 50);

// Получение высоты строки
double height = table.GetCellHeight(0);

// Установка высоты строки
table.SetCellHeight(0, 30, SizeMode.Exact);
```

### Работа с объединением
```csharp
// Объединение ячеек
table.MergeCells(0, 1);

// Разделение ячейки
table.SplitCell(0, 2, 3);
```

## Свойства таблицы

| Свойство | Тип | Описание |
|----------|-----|----------|
| `CellsCount` | `int` | Количество ячеек |
| `ColumnsCount` | `int` | Количество столбцов |
| `RowsCount` | `int` | Количество строк |
| `Properties` | `CellProperties` | Свойства по умолчанию |
| `CharFormat` | `CharFormat` | Формат символов по умолчанию |
| `ParagraphFormat` | `ParaFormat` | Формат абзацев по умолчанию |

## Перечисления

### Table.TextVAlign
Вертикальное выравнивание текста:
- `Top` - По верхнему краю
- `Center` - По центру
- `Bottom` - По нижнему краю

### Table.TextHAlign
Горизонтальное выравнивание текста:
- `Left` - По левому краю
- `Center` - По центру
- `Right` - По правому краю

### Table.TextDirection
Направление текста:
- `Normal` - Нормальное
- `BottomToTop` - Снизу вверх
- `TopToBottom` - Сверху вниз

### Table.TableHAlign
Выравнивание таблицы:
- `Left` - По левому краю
- `Center` - По центру
- `Right` - По правому краю

## Примеры использования

### Базовое создание таблицы
```csharp
Document document = TFlex.Application.ActiveDocument;
document.BeginChanges("Создание таблицы");

MultilineText mt = new MultilineText(document);
mt.BeginEdit();

Table.CreationSettings sett = new Table.CreationSettings(3, 2);
Table table = mt.CreateTable(sett);

table.InsertText(0, 0, "Ячейка 1");
table.InsertText(1, 0, "Ячейка 2");

mt.EndEdit();
document.EndChanges();
```

### Создание таблицы с настройками
```csharp
Table.CreationSettings sett = new Table.CreationSettings(3, 2);
Table.CellProperties prop = new Table.CellProperties();
prop.CellWidth = 30;
prop.RowHeight = 20;
prop.CellTextVAlign = Table.TextVAlign.Center;

Table table = mt.CreateTable(sett, prop);
```

### Работа со свойствами ячеек
```csharp
// Получение свойств
Table.CellProperties prop = table.GetCellProperties(0);

// Изменение свойств
prop.CellWidth = 40;
prop.BackgroundColor = 12632256; // Серый

// Установка свойств
table.SetCellProperties(0, prop);
```

### Объединение ячеек
```csharp
// Объединение ячеек 0 и 1
table.MergeCells(0, 1);
table.InsertText(0, 0, "Объединенная ячейка");

// Разделение ячейки
table.SplitCell(0, 2, 2);
```

## Рекомендации

### Обязательно используйте:
```csharp
document.BeginChanges("Описание");
// Ваши операции с таблицей
document.EndChanges();
```

### Проверяйте документ:
```csharp
if (TFlex.Application.ActiveDocument != null)
{
    Document document = TFlex.Application.ActiveDocument;
    // Работа с таблицей
}
```

### Обработка ошибок:
```csharp
try
{
    document.BeginChanges("Работа с таблицей");
    // Операции с таблицей
    document.EndChanges();
}
catch (Exception ex)
{
    document.CancelChanges();
    // Обработка ошибки
}
```

## Частые ошибки

1. ❌ Отсутствие блоков изменений
2. ❌ Некорректные индексы ячеек
3. ❌ Неправильное объединение ячеек
4. ❌ Превышение допустимых размеров таблицы

## Полезные ссылки

- `MultilineText` - многострочный текст
- `CharFormat` - формат символов
- `ParaFormat` - формат абзацев
- `SizeMode` - режимы размеров

---
*Шпаргалка создана на основе документации T-Flex CAD API*
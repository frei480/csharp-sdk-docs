# Шпаргалка по структуре Table в T-Flex CAD API

## Создание таблицы

```csharp
// Настройки таблицы
Table.CreationSettings settings = new Table.CreationSettings(3, 2); // 3 строки, 2 столбца

// Создание таблицы в текстовом блоке
Table table = paragraphText.CreateTable(settings);
```

## Основные свойства

| Свойство | Описание |
|---------|----------|
| `RowCount` | Количество строк |
| `ColumnCount` | Количество столбцов |
| `CellCount` | Количество ячеек |
| `IsRegular` | Регулярная таблица |
| `Properties` | Общие параметры |

## Работа с ячейками

### Получение текста
```csharp
// Получить текст ячейки
string text = table.GetCellText(0);

// Длина текста в ячейке
uint length = table.GetCellTextLength(0);
```

### Вставка текста
```csharp
// Вставить текст
table.InsertText(0, "Текст");

// Вставить форматированный текст
CharFormat format = new CharFormat
{
    Bold = true,
    FontSize = 3.5
};
table.InsertText(0, "Форматированный текст", format);
```

### Очистка ячейки
```csharp
// Очистить содержимое ячейки
table.Clear(0);
```

## Работа со строками и столбцами

### Вставка
```csharp
// Вставить строки
table.InsertRows(2, 0, Table.InsertProperties.After);

// Вставить столбцы
table.InsertColumns(1, 0, Table.InsertProperties.Before);
```

### Удаление
```csharp
// Удалить строку
table.DeleteRow(0);

// Удалить столбец
table.DeleteColumn(0);
```

## Объединение и разделение ячеек

### Объединение
```csharp
// Объединить ячейки
table.MergeCells(0, 3); // объединить ячейки с 0 по 3

// Объединить по координатам
table.MergeCells(0, 1, 0, 1); // объединить прямоугольник
```

### Разделение
```csharp
// Разделить ячейку
table.SplitCell(0, 2, 2); // разделить на 2 строки и 2 столбца
```

## Форматирование

### Параметры ячейки
```csharp
// Получить параметры
Table.CellProperties properties = table.GetCellProperties(0);

// Установить параметры
Table.CellProperties newProperties = new Table.CellProperties
{
    CellWidth = 50,
    RowHeight = 15,
    CellTextHAlign = Table.TextHAlign.Center,
    CellTextVAlign = Table.TextVAlign.Center,
    BackgroundColor = 15790320 // серый цвет
};
table.SetCellProperties(0, newProperties);
```

### Групповое форматирование
```csharp
// Установить параметры для группы ячеек
table.SetCellsProperties(0, 5, newProperties);
```

## Размеры и позиционирование

### Размеры ячеек
```csharp
// Получить ширину ячейки
double width = table.GetCellWidth(0);

// Установить ширину ячейки
table.SetCellWidth(0, 50);

// Получить высоту ячейки
double height = table.GetCellHeight(0);

// Установить высоту ячейки
table.SetCellHeight(0, 15);
```

### Прямоугольники ячеек
```csharp
// Получить прямоугольник ячейки
Rectangle rect = table.GetCellRectangle(0);
```

## Работа с выделением

```csharp
// Выделить всю таблицу
table.SelectAll();

// Выделить фрагмент
table.SetSelection(0, 5);

// Установить позицию курсора
table.SetCursorPosition(0);
```

## Границы ячеек

```csharp
// Настройка границ
Table.CellBorderProperties borders = new Table.CellBorderProperties(
    Table.CellBorderType.Thick,  // верхняя
    Table.CellBorderType.Thick,  // нижняя
    Table.CellBorderType.Thick,  // левая
    Table.CellBorderType.Thick   // правая
);

Table.CellProperties properties = new Table.CellProperties();
properties.CellBorder = borders;
table.SetCellProperties(0, properties);
```

## Типы выравнивания

### Горизонтальное выравнивание
- `Table.TextHAlign.Left` - По левому краю
- `Table.TextHAlign.Center` - По центру
- `Table.TextHAlign.Right` - По правому краю
- `Table.TextHAlign.Justify` - По ширине

### Вертикальное выравнивание
- `Table.TextVAlign.Top` - По верхнему краю
- `Table.TextVAlign.Center` - По центру
- `Table.TextVAlign.Bottom` - По нижнему краю

## Управление таблицей

### Удаление
```csharp
// Удалить таблицу
table.Delete();
```

### Получение позиции
```csharp
// Получить позицию таблицы в тексте
uint position = table.GetTablePosition();
```

## Частые ошибки

1. **Индекс вне диапазона**
   - Проверяйте `CellCount` перед обращением к ячейке

2. **Неправильное объединение**
   - Убедитесь, что ячейки не пересекаются с другими объединенными ячейками

3. **Неправильные размеры**
   - Проверяйте размеры ячеек при установке

## См. также
- [Document](DocumentCheatsheet.md)
- [ModelObject](ModelObjectCheatsheet.md)
- [ParagraphText](ParagraphTextCheatsheet.md)
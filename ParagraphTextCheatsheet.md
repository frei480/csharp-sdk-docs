# Шпаргалка по классу ParagraphText в T-Flex CAD API

## Создание текстового блока

```csharp
// Создание текстового блока
ParagraphText paragraphText = new ParagraphText(document);
paragraphText.X = 100;
paragraphText.Y = 100;
```

## Редактирование текста

### Основные методы
```csharp
// Начало редактирования
paragraphText.BeginEdit();

// Завершение редактирования
paragraphText.EndEdit();

// Очистка всего текста
paragraphText.ClearAll();

// Выделение всего текста
paragraphText.SelectAll();
```

### Вставка текста
```csharp
// Простой текст
paragraphText.InsertText("Текст");

// Форматированный текст
CharFormat format = new CharFormat
{
    FontName = "Arial",
    FontSize = 5.0,
    Bold = true
};
paragraphText.InsertText("Форматированный текст", format);
```

### Специальные символы
```csharp
// Разрыв строки
paragraphText.InsertCommonSymbol(CommonSymbol.LineBreak);

// Абзац
paragraphText.InsertParagraph();

// Индексы
paragraphText.InsertIndex("верхний", "нижний");
```

## Работа с таблицами

### Создание таблицы
```csharp
// Настройки таблицы
Table.CreationSettings settings = new Table.CreationSettings(3, 2);

// Создание таблицы
Table table = paragraphText.CreateTable(settings);
```

### Работа с таблицами
```csharp
// Первая таблица
Table firstTable = paragraphText.GetFirstTable();

// Следующая таблица
Table nextTable = paragraphText.GetNextTable();

// Таблица по индексу
Table table = paragraphText.GetTableByIndex(0);
```

## Форматирование

### Формат символов
```csharp
// Формат по умолчанию
CharFormat defaultFormat = new CharFormat
{
    FontName = "Arial",
    FontSize = 3.5,
    Color = 0
};
paragraphText.DefaultCharacterFormat = defaultFormat;

// Текущий формат
CharFormat currentFormat = paragraphText.CharacterFormat;
```

### Формат абзацев
```csharp
// Формат по умолчанию
ParaFormat defaultPara = new ParaFormat
{
    HorJustification = ParaFormat.Just.Left,
    LineSpaceMode = ParaFormat.LineSpaceSizeMode.Single
};
paragraphText.DefaultParagraphFormat = defaultPara;
```

## Работа с прямоугольниками

### Добавление прямоугольников
```csharp
// Создание прямоугольника
ParagraphText.TextRectangle rect = new ParagraphText.TextRectangle(
    new ParagraphText.TextRectangle.Point(10, 100),
    new ParagraphText.TextRectangle.Point(100, 50),
    document.GetPages().First(),
    0
);

// Добавление прямоугольника
paragraphText.AddRectangle(rect);
```

### Управление прямоугольниками
```csharp
// Количество прямоугольников
int count = paragraphText.GetRectanglesCount();

// Получение прямоугольника
ParagraphText.TextRectangle rect = paragraphText.GetRectangle(0);
```

## Управление размерами

### Действия при изменении размеров
```csharp
// Действие при увеличении высоты
paragraphText.HeightAction = ParagraphText.FitHeightAction.EnlargeDown;

// Действие при увеличении ширины
paragraphText.WidthAction = ParagraphText.FitWidthAction.EnlargeRight;

// Действие с пустым прямоугольником
paragraphText.EmptyRectangleAction = ParagraphText.EmptyRectAction.Delete;
```

## Работа с выделением

### Управление выделением
```csharp
// Снять выделение
paragraphText.Deselect();

// Получить границы выделения
Position start, end;
paragraphText.GetSelection(out start, out end);

// Установить выделение
paragraphText.SetSelection(start, end);
```

## Позиционирование курсора

```csharp
// Установить позицию курсора
paragraphText.SetCursor(new PositionProperties(0));

// Переместить курсор
paragraphText.MoveCursor(5); // на 5 символов вперед
paragraphText.MoveCursor(-3); // на 3 символа назад
```

## Полезные свойства

| Свойство | Описание |
|---------|----------|
| `TextLength` | Длина текста |
| `TextValue` | Значение текста |
| `BoundRect` | Ограничивающий прямоугольник |
| `AutoUpdate` | Автоматическое обновление |
| `Page` | Страница размещения |

## Частые ошибки

1. **Забытое BeginEdit()**
   - Всегда вызывайте BeginEdit() перед вставкой текста

2. **Неправильные координаты прямоугольников**
   - Проверяйте порядок координат (левая верхняя, правая нижняя)

3. **Превышение индексов**
   - Проверяйте количество прямоугольников перед доступом

## См. также
- [Document](DocumentCheatsheet.md)
- [ModelObject](ModelObjectCheatsheet.md)
- [Table](TableCheatsheet.md)
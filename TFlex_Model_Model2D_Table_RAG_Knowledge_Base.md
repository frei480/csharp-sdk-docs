# База знаний по классу TFlex.Model.Model2D.Table для RAG-системы

## Общая информация

Класс `Table` в T-Flex CAD API представляет собой таблицу, которая может быть вставлена в многострочный текст (`MultilineText`). Это мощный инструмент для создания структурированного текстового контента в чертежах.

### Назначение класса
- Создание таблиц в многострочном тексте
- Управление структурой таблицы (строки, столбцы, ячейки)
- Форматирование содержимого таблицы
- Работа с объединенными ячейками

### Иерархия наследования
```
System.Object
  TFlex.Model.Model2D.Table
```

## Основные компоненты

### Table.CreationSettings
Класс для настройки параметров создания таблицы.

**Свойства:**
- `ColumnsCount` (int) - Количество столбцов
- `RowsCount` (int) - Количество строк

**Конструктор:**
```csharp
Table.CreationSettings(int columns, int rows)
```

### Table.CellProperties
Класс для управления свойствами ячеек таблицы.

**Свойства:**
- `CellWidth` (double) - Ширина ячейки
- `RowHeight` (double) - Высота строки
- `CellTextVAlign` (Table.TextVAlign) - Вертикальное выравнивание текста
- `CellTextHAlign` (Table.TextHAlign) - Горизонтальное выравнивание текста
- `TextDirection` (Table.TextDirection) - Направление текста
- `BackgroundColor` (int) - Цвет фона ячейки
- `RowHeightMode` (SizeMode) - Режим размера строки
- `CellWidthMode` (SizeMode) - Режим размера ячейки
- `RowWrap` (bool) - Перенос текста в строке

### Table.InsertProperties
Перечисление для определения позиции вставки строк/столбцов.

**Значения:**
- `Before` - Перед указанной ячейкой
- `After` - После указанной ячейки

## Основные методы класса Table

### Создание и настройка таблицы

#### CreateTable(CreationSettings settings)
Создает таблицу с заданными настройками.

**Параметры:**
- `settings` (Table.CreationSettings) - Настройки создания таблицы

**Возвращает:**
- `Table` - Созданная таблица

#### CreateTable(CreationSettings settings, CellProperties properties)
Создает таблицу с заданными настройками и свойствами ячеек.

**Параметры:**
- `settings` (Table.CreationSettings) - Настройки создания таблицы
- `properties` (Table.CellProperties) - Свойства ячеек

**Возвращает:**
- `Table` - Созданная таблица

### Работа с ячейками

#### GetCellProperties(int cellIndex)
Получает свойства ячейки по индексу.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки

**Возвращает:**
- `Table.CellProperties` - Свойства ячейки

#### SetCellProperties(int cellIndex, CellProperties properties)
Устанавливает свойства ячейки по индексу.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки
- `properties` (Table.CellProperties) - Свойства ячейки

#### GetCellText(int cellIndex)
Получает текст из ячейки.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки

**Возвращает:**
- `string` - Текст ячейки

#### GetCellText(int cellIndex, bool withBraces)
Получает текст из ячейки с символами форматирования.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки
- `withBraces` (bool) - Включать символы форматирования

**Возвращает:**
- `string` - Текст ячейки

#### InsertText(int cellIndex, int charIndex, string text)
Вставляет текст в ячейку.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки
- `charIndex` (int) - Индекс символа для вставки
- `text` (string) - Текст для вставки

#### InsertText(int cellIndex, int charIndex, string text, CharFormat format)
Вставляет текст в ячейку с заданным форматом.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки
- `charIndex` (int) - Индекс символа для вставки
- `text` (string) - Текст для вставки
- `format` (CharFormat) - Формат текста

#### Clear(int cellIndex)
Очищает содержимое ячейки.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки

### Управление структурой таблицы

#### InsertRows(int cellIndex, int count, Table.InsertProperties position)
Вставляет строки в таблицу.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки, относительно которой вставляются строки
- `count` (int) - Количество строк для вставки
- `position` (Table.InsertProperties) - Позиция вставки

#### InsertColumns(int cellIndex, int count, Table.InsertProperties position)
Вставляет столбцы в таблицу.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки, относительно которой вставляются столбцы
- `count` (int) - Количество столбцов для вставки
- `position` (Table.InsertProperties) - Позиция вставки

#### DeleteRow(int cellIndex)
Удаляет строку, содержащую указанную ячейку.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки в строке для удаления

#### DeleteColumn(int cellIndex)
Удаляет столбец, содержащий указанную ячейку.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки в столбце для удаления

### Работа с размерами

#### GetCellWidth(int cellIndex)
Получает ширину ячейки.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки

**Возвращает:**
- `double` - Ширина ячейки

#### SetCellWidth(int cellIndex, double width)
Устанавливает ширину ячейки.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки
- `width` (double) - Ширина ячейки

#### GetCellHeight(int cellIndex)
Получает высоту строки, содержащей ячейку.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки

**Возвращает:**
- `double` - Высота строки

#### SetCellHeight(int cellIndex, double height, SizeMode mode)
Устанавливает высоту строки, содержащей ячейку.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки
- `height` (double) - Высота строки
- `mode` (SizeMode) - Режим размера

### Работа с объединением ячеек

#### MergeCells(int firstCellIndex, int lastCellIndex)
Объединяет ячейки.

**Параметры:**
- `firstCellIndex` (int) - Индекс первой ячейки
- `lastCellIndex` (int) - Индекс последней ячейки

#### SplitCell(int cellIndex, int rows, int columns)
Разделяет объединенную ячейку.

**Параметры:**
- `cellIndex` (int) - Индекс ячейки для разделения
- `rows` (int) - Количество строк после разделения
- `columns` (int) - Количество столбцов после разделения

## Свойства класса Table

### Основные свойства

#### CellsCount (int)
Количество ячеек в таблице.

#### ColumnsCount (int)
Количество столбцов в таблице.

#### RowsCount (int)
Количество строк в таблице.

#### Properties (Table.CellProperties)
Свойства таблицы по умолчанию.

#### CharFormat (CharFormat)
Формат символов таблицы по умолчанию.

#### ParagraphFormat (ParaFormat)
Формат абзацев таблицы по умолчанию.

## Перечисления

### Table.TextVAlign
Вертикальное выравнивание текста в ячейке.

**Значения:**
- `Top` - По верхнему краю
- `Center` - По центру
- `Bottom` - По нижнему краю

### Table.TextHAlign
Горизонтальное выравнивание текста в ячейке.

**Значения:**
- `Left` - По левому краю
- `Center` - По центру
- `Right` - По правому краю

### Table.TextDirection
Направление текста в ячейке.

**Значения:**
- `Normal` - Нормальное направление
- `BottomToTop` - Снизу вверх
- `TopToBottom` - Сверху вниз

### Table.TableHAlign
Горизонтальное выравнивание таблицы.

**Значения:**
- `Left` - По левому краю
- `Center` - По центру
- `Right` - По правому краю

## Практическое применение

### Типичные сценарии использования

1. **Создание спецификаций**
   - Таблицы с параметрами деталей
   - Таблицы материалов
   - Таблицы стандартных изделий

2. **Оформление чертежей**
   - Титульные листы
   - Таблицы параметров
   - Таблицы допусков

3. **Создание отчетов**
   - Таблицы результатов расчетов
   - Таблицы измерений
   - Таблицы характеристик

### Интеграция с другими объектами

1. **С многострочным текстом (MultilineText)**
   - Таблицы как часть текстового содержимого
   - Комбинирование текста и таблиц

2. **С форматированием текста (CharFormat)**
   - Различные стили текста в ячейках
   - Форматирование заголовков таблиц

3. **С форматированием абзацев (ParaFormat)**
   - Выравнивание таблицы на странице
   - Отступы и интервалы

## Примеры кода

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
table.InsertText(2, 0, "Ячейка 3");

mt.EndEdit();
document.EndChanges();
```

### Работа со свойствами ячеек
```csharp
// Создание свойств ячейки
Table.CellProperties prop = new Table.CellProperties();
prop.CellWidth = 30;
prop.RowHeight = 20;
prop.CellTextVAlign = Table.TextVAlign.Center;
prop.CellTextHAlign = Table.TextHAlign.Center;
prop.BackgroundColor = 12632256; // Серый цвет

// Применение свойств к ячейке
table.SetCellProperties(0, prop);
```

### Объединение ячеек
```csharp
// Объединение ячеек с индексами 0 и 1
table.MergeCells(0, 1);
table.InsertText(0, 0, "Объединенная ячейка");
```

## Рекомендации по использованию

### Лучшие практики

1. **Всегда используйте блоки изменений**
   ```csharp
   document.BeginChanges("Описание операции");
   // Операции с таблицей
   document.EndChanges();
   ```

2. **Проверяйте существование документа**
   ```csharp
   if (TFlex.Application.ActiveDocument != null)
   {
       // Работа с таблицей
   }
   ```

3. **Используйте осмысленные имена переменных**
   - `specificationTable` вместо `table`
   - `headerCellProperties` вместо `prop`

4. **Управляйте ресурсами**
   - Не создавайте лишние объекты
   - Переиспользуйте существующие настройки

### Распространенные ошибки

1. **Отсутствие блоков изменений**
   - Приводит к некорректной работе с документом
   - Может вызвать исключения

2. **Некорректные индексы ячеек**
   - Выход за пределы допустимых значений
   - Отрицательные индексы

3. **Неправильное объединение ячеек**
   - Попытка объединить непоследовательные ячейки
   - Объединение уже объединенных ячеек

## Производительность

### Оптимизация работы с большими таблицами
```csharp
document.BeginChanges("Создание большой таблицы");
try
{
    Table.CreationSettings sett = new Table.CreationSettings(10, 20);
    Table table = mt.CreateTable(sett);
    
    // Пакетное заполнение таблицы
    Table.CellProperties defaultProp = new Table.CellProperties();
    defaultProp.CellWidth = 25;
    defaultProp.RowHeight = 15;
    
    for (int i = 0; i < 200; i++)
    {
        table.SetCellProperties(i, defaultProp);
        table.InsertText(i, 0, "Данные " + i);
    }
    
    document.EndChanges();
}
catch
{
    document.CancelChanges();
    throw;
}
```

### Рекомендации по производительности
- Группируйте операции в одном блоке изменений
- Используйте предварительное создание настроек
- Избегайте частых операций обновления экрана
- Удаляйте временные объекты после использования

## Совместимость и ограничения

### Ограничения API
- Максимальный размер таблицы ограничен памятью системы
- Некоторые комбинации объединения ячеек могут быть неподдерживаемыми
- Ограниченная поддержка сложного форматирования

### Совместимость с версиями
- Версия API: 17.1.20.0
- Совместимость с T-FLEX CAD 17.x

## Дополнительные ресурсы

### Связанные классы
- `MultilineText` - многострочный текст
- `CharFormat` - формат символов
- `ParaFormat` - формат абзацев
- `SizeMode` - режимы размеров

### Полезные перечисления
- `Table.TextVAlign` - вертикальное выравнивание текста
- `Table.TextHAlign` - горизонтальное выравнивание текста
- `Table.TextDirection` - направление текста
- `Table.TableHAlign` - выравнивание таблицы

Эта база знаний предоставляет исчерпывающую информацию о классе `TFlex.Model.Model2D.Table` для использования в RAG-системе, включая все аспекты его применения, интеграции и оптимизации.
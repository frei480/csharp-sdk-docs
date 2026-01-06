# Примеры использования классов в пространстве имён TFlex.Dialogs

## Описание пространства имён

Пространство имён `TFlex.Dialogs` содержит классы для создания и управления диалоговыми окнами в T-Flex CAD.

## Основные классы

### ModalDialog

Базовый класс для модальных диалоговых окон.

**Пример создания простого диалога:**
```csharp
internal class SimpleDialog : ModalDialog
{
    public SimpleDialog() : base("Мой диалог")
    {
        // Создание страницы диалога
        ModalDialogPage page = new ModalDialogPage();
        Pages.Add(page);
        
        // Добавление элементов управления
        GridControl grid = new GridControl { RowCount = 2, ColumnCount = 1 };
        page.Controls.Add(grid);
        
        // Добавление кнопки
        ToggleControl checkBox = new ToggleControl() { Text = "Включить опцию" };
        grid.SetControl(0, 0, checkBox);
        
        // Добавление числового поля
        NumericInputControl numberInput = new NumericInputControl() { Value = 10.0 };
        grid.SetControl(1, 0, numberInput);
    }
}
```

**Пример показа диалога:**
```csharp
SimpleDialog dialog = new SimpleDialog();
bool result = dialog.ShowDialog();

if (result)
{
    // Пользователь нажал OK
    // Обработка введенных данных
}
else
{
    // Пользователь нажал Cancel или закрыл диалог
}
```

### ModalDialogPage

Класс представляет страницу в модальном диалоге (для многостраничных диалогов).

**Пример создания многостраничного диалога:**
```csharp
internal class MultiPageDialog : ModalDialog
{
    public MultiPageDialog() : base("Многостраничный диалог")
    {
        // Первая страница
        ModalDialogPage page1 = new ModalDialogPage();
        page1.Caption = "Основные настройки";
        // Добавление элементов...
        Pages.Add(page1);
        
        // Вторая страница
        ModalDialogPage page2 = new ModalDialogPage();
        page2.Caption = "Дополнительные параметры";
        // Добавление элементов...
        Pages.Add(page2);
    }
}
```

### GridControl

Класс для создания сетки элементов управления.

**Пример создания сетки:**
```csharp
GridControl grid = new GridControl();
grid.RowCount = 3;
grid.ColumnCount = 2;

// Установка автоматической ширины для столбца
grid.SetAutoWidth(0);

// Добавление элементов
ToggleControl check1 = new ToggleControl() { Text = "Опция 1" };
grid.SetControl(0, 0, check1);

ToggleControl check2 = new ToggleControl() { Text = "Опция 2" };
grid.SetControl(0, 1, check2);

NumericInputControl input1 = new NumericInputControl() { Value = 5.0 };
grid.SetControl(1, 0, input1);

NumericInputControl input2 = new NumericInputControl() { Value = 10.0 };
grid.SetControl(1, 1, input2);

// Добавление в диалог
dialogPage.Controls.Add(grid);
```

### ControlsWindowForm

Класс для создания форм с элементами управления.

**Пример использования:**
```csharp
ControlsWindowForm form = new ControlsWindowForm();
form.Caption = "Параметры модели";

// Добавление сетки элементов
GridControl grid = new GridControl { RowCount = 2, ColumnCount = 1 };
form.Controls.Add(grid);

// Добавление в страницу диалога
dialogPage.Controls.Add(form);
```

### CheckState

Перечисление состояний флажков.

**Примеры использования:**
```csharp
// Установка состояния флажка
ToggleControl checkBox = new ToggleControl();
checkBox.CheckState = CheckState.Checked;    // Отмечен
checkBox.CheckState = CheckState.Unchecked;  // Не отмечен
checkBox.CheckState = CheckState.Indeterminate; // Неопределенное состояние

// Проверка состояния
if (checkBox.CheckState == CheckState.Checked)
{
    // Флажок отмечен
}
```

### ToggleControl

Класс для элементов управления с двумя состояниями (флажки).

**Пример создания и настройки:**
```csharp
ToggleControl dynamicPreviewCheck = new ToggleControl() 
{ 
    Text = "Динамический предварительный просмотр",
    CheckState = CheckState.Checked 
};

// Обработка изменения состояния
dynamicPreviewCheck.CheckStateChanged += (sender, e) =>
{
    bool isEnabled = (sender as ToggleControl).CheckState == CheckState.Checked;
    // Включение/отключение динамического просмотра
};
```

### NumericInputControl

Класс для ввода числовых значений.

**Пример создания поля ввода:**
```csharp
NumericInputControl lengthInput = new NumericInputControl();
lengthInput.Caption = "Длина";
lengthInput.Value = 100.0;
lengthInput.Minimum = 0.0;
lengthInput.Maximum = 1000.0;
lengthInput.Step = 1.0;

// Обработка изменения значения
lengthInput.ValueChanged += (sender, e) =>
{
    double newLength = (sender as NumericInputControl).Value;
    // Обновление модели с новой длиной
};
```

### TabControl

Класс для создания вкладок в диалоговом окне.

**Пример создания вкладок:**
```csharp
TabControl tabControl = new TabControl();

// Создание вкладок
ControlsWindowForm generalTab = new ControlsWindowForm { Caption = "Общие" };
ControlsWindowForm advancedTab = new ControlsWindowForm { Caption = "Дополнительно" };

// Добавление элементов на вкладки
// ... 

// Добавление вкладок в TabControl
tabControl.AddTab(generalTab);
tabControl.AddTab(advancedTab);

// Добавление в диалог
dialogPage.Controls.Add(tabControl);
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Dialogs_Examples.md
# Шпаргалка по классам в пространстве имён TFlex.Dialogs

## ModalDialog
| Метод/Свойство | Тип | Описание |
|---|---|---|
| Caption | string | Заголовок диалога |
| Pages | Collection | Страницы диалога |
| ShowDialog() | bool | Показать диалог |
| ModalDialog(caption) | Конструктор | Создание диалога |

## ModalDialogPage
| Свойство | Тип | Описание |
|---|---|---|
| Caption | string | Заголовок страницы |
| Controls | Collection | Элементы управления |
| Visible | bool | Видимость |

## GridControl
| Свойство/Метод | Тип | Описание |
|---|---|---|
| RowCount | int | Количество строк |
| ColumnCount | int | Количество столбцов |
| SetControl(row,col,ctrl) | void | Разместить элемент |
| SetAutoWidth(col) | void | Автоширина столбца |

## ControlsWindowForm
| Свойство | Тип | Описание |
|---|---|---|
| Caption | string | Заголовок группы |
| Controls | Collection | Дочерние элементы |

## CheckState
- Unchecked - не отмечено
- Checked - отмечено
- Indeterminate - неопределено

## ToggleControl
| Свойство/Событие | Тип | Описание |
|---|---|---|
| Text | string | Текст флажка |
| CheckState | CheckState | Состояние |
| Enabled | bool | Доступность |
| CheckStateChanged | Event | Изменение состояния |

## NumericInputControl
| Свойство/Событие | Тип | Описание |
|---|---|---|
| Value | double | Значение |
| Minimum | double | Мин. значение |
| Maximum | double | Макс. значение |
| Step | double | Шаг |
| Caption | string | Заголовок |
| Enabled | bool | Доступность |
| ValueChanged | Event | Изменение значения |

## TabControl
| Метод | Параметры | Описание |
|---|---|---|
| AddTab(tab) | ControlsWindowForm | Добавить вкладку |

## Быстрые примеры

```csharp
// Диалог
class MyDialog : ModalDialog {
    public MyDialog() : base("Мой диалог") {
        var page = new ModalDialogPage();
        Pages.Add(page);
        
        var grid = new GridControl { RowCount = 2, ColumnCount = 1 };
        page.Controls.Add(grid);
        
        var check = new ToggleControl { Text = "Опция" };
        grid.SetControl(0, 0, check);
        
        var input = new NumericInputControl { Value = 10.0 };
        grid.SetControl(1, 0, input);
    }
}

// Использование
var dialog = new MyDialog();
if (dialog.ShowDialog()) {
    // OK
}
```

## Шаблоны диалогов

```csharp
// Простой диалог с одним параметром
class SimpleParamDialog : ModalDialog {
    NumericInputControl input;
    
    public SimpleParamDialog(string title, double defaultValue) : base(title) {
        var page = new ModalDialogPage();
        Pages.Add(page);
        
        var grid = new GridControl { RowCount = 1, ColumnCount = 1 };
        page.Controls.Add(grid);
        
        input = new NumericInputControl { Value = defaultValue };
        grid.SetControl(0, 0, input);
    }
    
    public double Value => input.Value;
}

// Диалог с флажками
class OptionsDialog : ModalDialog {
    ToggleControl opt1, opt2;
    
    public OptionsDialog() : base("Опции") {
        // ... создание элементов
    }
    
    public bool Option1 => opt1.CheckState == CheckState.Checked;
    public bool Option2 => opt2.CheckState == CheckState.Checked;
}
```

## Обработка событий

```csharp
// Валидация ввода
input.ValueChanged += (s, e) => {
    var ctrl = s as NumericInputControl;
    if (ctrl.Value < 0) {
        ctrl.Value = 0;
        MessageBox.Show("Значение не может быть отрицательным");
    }
};

// Динамическое включение
check.CheckStateChanged += (s, e) => {
    input.Enabled = (s as ToggleControl).CheckState == CheckState.Checked;
};
```

## Типичные ошибки
- Забывание `grid.SetAutoWidth(0)`
- Неправильные индексы в `SetControl`
- Отсутствие проверки `ShowDialog()` результата
- Блокировка UI в обработчиках событий</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Dialogs_Cheat_Sheet.md
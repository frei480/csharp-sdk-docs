# Шпаргалка по классам в пространстве имён TFlex.Command

## Plugin
| Метод | Описание |
|---|---|
| OnInitialize() | Инициализация плагина |
| OnCreateTools() | Создание команд и UI |
| OnCommand(doc, id) | Обработка команд |
| RegisterCommand(id, name, icon, icon) | Регистрация команды |
| RegisterObjectTypeIcon(id, icon) | Регистрация иконки типа |

## Application
| Свойство/Метод | Тип | Описание |
|---|---|---|
| ActiveDocument | Document | Текущий документ |
| Version | Version | Версия приложения |
| OpenDocument(path) | Document | Открыть документ |
| GetCustomLicenseStatus(id) | bool | Проверить лицензию |
| InitializeCustomLicense(id) | void | Инициализировать лицензию |

## Menu
| Метод | Параметры | Описание |
|---|---|---|
| CreatePopup() | void | Создать всплывающее меню |
| Append(cmdId, text, plugin) | void | Добавить команду |
| AppendSeparator() | void | Добавить разделитель |
| AppendSubMenu(text, menu) | void | Добавить подменю |

## MainWindow
| Метод | Описание |
|---|---|
| InsertPluginSubMenu(name, menu, pos, plugin) | Вставить меню плагина |

## DocumentEventArgs
| Свойство | Тип | Описание |
|---|---|---|
| Document | Document | Документ события |

## LibraryConfigurations
| Свойство/Метод | Тип | Описание |
|---|---|---|
| Active | LibraryConfiguration | Активная библиотека |
| Count | int | Количество библиотек |
| Open(path) | void | Открыть библиотеку |

## LibraryConfiguration
| Свойство/Метод | Тип | Описание |
|---|---|---|
| Name | string | Имя библиотеки |
| Path | string | Путь к файлу |
| IsActive | bool | Активна ли |
| Activate() | void | Активировать |
| Close() | void | Закрыть |

## Быстрые примеры

```csharp
// Плагин
public class MyPlugin : TFlex.Plugin {
    public MyPlugin(Factory f) : base(f) {}
    
    protected override void OnCreateTools() {
        RegisterCommand(1, "Команда", null, null);
        
        var menu = new TFlex.Menu();
        menu.CreatePopup();
        menu.Append(1, "Команда", this);
        
        Application.ActiveMainWindow.InsertPluginSubMenu("Плагин", menu, 
            TFlex.MainWindow.InsertMenuPosition.EndOfTools, this);
    }
    
    protected override void OnCommand(Document doc, int id) {
        if (id == 1) {
            // Выполнить команду
        }
    }
}

// Лицензия
if (!TFlex.Application.GetCustomLicenseStatus(12)) return;
TFlex.Application.InitializeCustomLicense(12);

// Библиотеки
var libs = new LibraryConfigurations();
libs.Open("library.tws");
var activeLib = libs.Active;
```

## Шаблон плагина

```csharp
public class TemplatePlugin : TFlex.Plugin {
    public TemplatePlugin(Factory f) : base(f) {}
    
    protected override void OnInitialize() {
        base.OnInitialize();
        TFlex.Application.InitializeCustomLicense(123);
    }
    
    protected override void OnCreateTools() {
        base.OnCreateTools();
        RegisterCommands();
        CreateMenus();
        CreateRibbon();
    }
    
    protected override void OnCommand(Document doc, int id) {
        try {
            ExecuteCommand(doc, id);
        } catch (Exception ex) {
            HandleError(ex);
        }
    }
    
    private void RegisterCommands() { }
    private void CreateMenus() { }
    private void CreateRibbon() { }
    private void ExecuteCommand(Document doc, int id) { }
    private void HandleError(Exception ex) { }
}
```

## События

```csharp
// Открытие документа
protected override void DocumentOpenEventHandler(DocumentEventArgs e) {
    e.Document.AttachPlugin(this);
}

// Создание документа
protected override void NewDocumentCreatedEventHandler(DocumentEventArgs e) {
    InitializeDocument(e.Document);
}
```

## Типичные ошибки
- Отсутствие проверки лицензии
- Неправильные ID команд
- Забывание base.OnInitialize()
- Блокировка UI в OnCommand()
- Отсутствие обработки исключений</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Command_Cheat_Sheet.md
# Примеры использования классов в пространстве имён TFlex.Command

## Описание пространства имён

Пространство имён `TFlex.Command` содержит классы для создания команд, плагинов и интеграции с интерфейсом T-Flex CAD.

## Основные классы

### Plugin

Базовый класс для создания плагинов T-Flex CAD.

**Пример создания плагина:**
```csharp
public class MyPlugin : TFlex.Plugin
{
    public MyPlugin(Factory factory) : base(factory)
    {
    }

    protected override void OnInitialize()
    {
        base.OnInitialize();
        // Инициализация плагина
    }

    protected override void OnCreateTools()
    {
        base.OnCreateTools();
        
        // Регистрация команд
        RegisterCommand((int)Commands.MyCommand, "Моя команда", null, null);
        
        // Создание меню
        TFlex.Menu menu = new TFlex.Menu();
        menu.CreatePopup();
        menu.Append((int)Commands.MyCommand, "Моя команда", this);
        
        // Добавление меню в интерфейс
        Application.ActiveMainWindow.InsertPluginSubMenu("Мой плагин", menu, 
            TFlex.MainWindow.InsertMenuPosition.EndOfTools, this);
    }

    protected override void OnCommand(Document document, int cmdId)
    {
        switch ((Commands)cmdId)
        {
            case Commands.MyCommand:
                // Выполнение команды
                ExecuteMyCommand(document);
                break;
        }
    }
}
```

### Application

Класс предоставляет доступ к основным функциям приложения T-Flex CAD.

**Пример работы с приложением:**
```csharp
// Получение активного документа
Document activeDoc = TFlex.Application.ActiveDocument;

// Получение версии приложения
Version appVersion = TFlex.Application.Version;

// Открытие документа
Document newDoc = TFlex.Application.OpenDocument("path/to/file.grb");

// Проверка лицензии
bool hasLicense = TFlex.Application.GetCustomLicenseStatus(12);

// Инициализация лицензии
TFlex.Application.InitializeCustomLicense(12);
```

### Menu

Класс для создания меню и контекстных меню.

**Пример создания меню:**
```csharp
TFlex.Menu mainMenu = new TFlex.Menu();
mainMenu.CreatePopup();

// Добавление команд
mainMenu.Append((int)Commands.Create, "Создать", this);
mainMenu.Append((int)Commands.Edit, "Редактировать", this);
mainMenu.AppendSeparator(); // Разделитель
mainMenu.Append((int)Commands.Delete, "Удалить", this);

// Добавление подменю
TFlex.Menu subMenu = new TFlex.Menu();
subMenu.CreatePopup();
subMenu.Append((int)Commands.SubCommand1, "Подкоманда 1", this);
mainMenu.AppendSubMenu("Подменю", subMenu);
```

### MainWindow

Класс предоставляет доступ к главному окну приложения.

**Пример работы с главным окном:**
```csharp
// Добавление меню плагина
Application.ActiveMainWindow.InsertPluginSubMenu("Мой плагин", menu, 
    TFlex.MainWindow.InsertMenuPosition.EndOfTools, this);

// Добавление кнопок на панель инструментов
// (зависит от версии T-Flex)

// Получение активного вида
View activeView = Application.ActiveMainWindow.ActiveView;
```

### DocumentEventArgs

Класс аргументов событий документа.

**Пример обработки событий документа:**
```csharp
protected override void DocumentOpenEventHandler(DocumentEventArgs args)
{
    // Документ открыт
    Document doc = args.Document;
    
    // Присоединение плагина к документу
    doc.AttachPlugin(this);
    
    // Инициализация для нового документа
    InitializeForDocument(doc);
}

protected override void NewDocumentCreatedEventHandler(DocumentEventArgs args)
{
    // Создан новый документ
    SetupNewDocument(args.Document);
}
```

### LibraryConfigurations

Класс для управления конфигурациями библиотек.

**Пример работы с библиотеками:**
```csharp
LibraryConfigurations libs = new LibraryConfigurations();

// Получение активной библиотеки
LibraryConfiguration activeLib = libs.Active;

// Перебор всех библиотек
foreach (LibraryConfiguration lib in libs)
{
    Console.WriteLine($"Библиотека: {lib.Name}");
    Console.WriteLine($"Путь: {lib.Path}");
}

// Открытие новой библиотеки
libs.Open(@"C:\Libraries\MyLibrary.tws");

// Поиск библиотеки по имени
LibraryConfiguration foundLib = null;
foreach (LibraryConfiguration lib in libs)
{
    if (lib.Name == "Мои элементы")
    {
        foundLib = lib;
        break;
    }
}
```

### LibraryConfiguration

Класс представляет отдельную конфигурацию библиотеки.

**Пример работы с конфигурацией:**
```csharp
LibraryConfiguration lib = libs.Active;

// Свойства библиотеки
string name = lib.Name;
string path = lib.Path;
bool isActive = lib.IsActive;

// Активация библиотеки
lib.Activate();

// Закрытие библиотеки
lib.Close();
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Command_Examples.md
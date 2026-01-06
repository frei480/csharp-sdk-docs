# Продвинутые примеры использования классов в пространстве имён TFlex.Command

## Комплексная разработка плагинов

### Создание полнофункционального плагина для работы с валами

```csharp
public class ShaftPlugin : TFlex.Plugin
{
    private const string RIBBON_GUID = "c5ed7f66-53e0-4847-bc6b-9d457f0014eb";
    
    public ShaftPlugin(Factory factory) : base(factory)
    {
    }

    protected override void OnInitialize()
    {
        base.OnInitialize();
        
        // Инициализация лицензии
        TFlex.Application.InitializeCustomLicense(12);
        
        // Проверка версии
        Version minVersion = new Version(17, 0);
        if (TFlex.Application.Version < minVersion)
        {
            throw new InvalidOperationException("Требуется T-Flex CAD 17.0 или выше");
        }
    }

    protected override void OnCreateTools()
    {
        base.OnCreateTools();

        // Регистрация команд
        RegisterCommand((int)ShaftCommands.CreateShaft, "Создать вал", 
            LoadIcon("CreateShaft"), LoadIcon("CreateShaft"));
        RegisterCommand((int)ShaftCommands.EditShaft, "Редактировать вал",
            LoadIcon("EditShaft"), LoadIcon("EditShaft"));
        RegisterCommand((int)ShaftCommands.DrawShaft, "Чертеж вала",
            LoadIcon("DrawShaft"), LoadIcon("DrawShaft"));

        // Создание главного меню
        CreateMainMenu();
        
        // Создание интерфейса ленты
        CreateRibbonInterface();
        
        // Регистрация типов объектов
        RegisterObjectTypeIcon((int)ObjectTypes.Shaft, LoadIcon("Shaft"));
    }

    private void CreateMainMenu()
    {
        TFlex.Menu shaftMenu = new TFlex.Menu();
        shaftMenu.CreatePopup();
        
        shaftMenu.Append((int)ShaftCommands.CreateShaft, "Создать вал", this);
        shaftMenu.Append((int)ShaftCommands.EditShaft, "Редактировать вал", this);
        shaftMenu.Append((int)ShaftCommands.DrawShaft, "Создать чертеж", this);
        
        // Добавление разделителя и дополнительных команд
        shaftMenu.AppendSeparator();
        shaftMenu.Append((int)ShaftCommands.Settings, "Настройки", this);
        shaftMenu.Append((int)ShaftCommands.Help, "Справка", this);

        Application.ActiveMainWindow.InsertPluginSubMenu("Валы", shaftMenu, 
            TFlex.MainWindow.InsertMenuPosition.EndOfTools, this);
    }

    private void CreateRibbonInterface()
    {
        try
        {
            var ribbonTab = new RibbonTab("Валы", new Guid(RIBBON_GUID), this);
            
            // Группа основных команд
            RibbonGroup mainGroup = ribbonTab.AddGroup("Основные");
            mainGroup.AddButton((int)ShaftCommands.CreateShaft, "Создать вал", this);
            mainGroup.AddButton((int)ShaftCommands.EditShaft, "Редактировать", this);
            
            // Группа дополнительных команд
            RibbonGroup advancedGroup = ribbonTab.AddGroup("Дополнительно");
            advancedGroup.AddButton((int)ShaftCommands.DrawShaft, "Чертеж", this);
            advancedGroup.AddButton((int)ShaftCommands.Analyze, "Анализ", this);
        }
        catch (Exception ex)
        {
            // Обработка ошибок создания ленты
            Console.WriteLine("Ошибка создания интерфейса ленты: " + ex.Message);
        }
    }

    protected override void OnCommand(Document document, int cmdId)
    {
        // Проверка лицензии
        if (!TFlex.Application.GetCustomLicenseStatus(12))
        {
            MessageBox.Show("Отсутствует лицензия для плагина валов");
            return;
        }

        // Проверка версии документа
        if (!CheckDocumentVersion(document))
        {
            return;
        }

        // Добавление библиотеки если необходимо
        EnsureLibraryLoaded();

        try
        {
            switch ((ShaftCommands)cmdId)
            {
                case ShaftCommands.CreateShaft:
                    ExecuteCreateShaft(document);
                    break;
                    
                case ShaftCommands.EditShaft:
                    ExecuteEditShaft(document);
                    break;
                    
                case ShaftCommands.DrawShaft:
                    ExecuteDrawShaft(document);
                    break;
                    
                case ShaftCommands.Settings:
                    ShowSettingsDialog();
                    break;
                    
                case ShaftCommands.Help:
                    ShowHelp();
                    break;
            }
        }
        catch (Exception ex)
        {
            HandleCommandError(ex);
        }
    }

    protected override void DocumentOpenEventHandler(DocumentEventArgs args)
    {
        base.DocumentOpenEventHandler(args);
        
        // Инициализация для открытого документа
        InitializeDocument(args.Document);
    }

    protected override void NewDocumentCreatedEventHandler(DocumentEventArgs args)
    {
        base.NewDocumentCreatedEventHandler(args);
        
        // Настройка нового документа
        SetupNewDocument(args.Document);
    }

    // Вспомогательные методы
    private void ExecuteCreateShaft(Document document)
    {
        var command = new CreateShaftCommand(this, document, false);
        command.Run(document.ActiveView);
    }

    private void ExecuteEditShaft(Document document)
    {
        if (document.Selection.Count == 0)
        {
            MessageBox.Show("Выберите вал для редактирования");
            return;
        }

        var selectedObject = document.Selection.GetAt(0);
        var command = new EditShaftCommand(this, selectedObject, document, false);
        
        if (!command.StopEditing)
        {
            command.Run(document.ActiveView);
        }
    }

    private void ExecuteDrawShaft(Document document)
    {
        // Реализация создания чертежа
    }

    private bool CheckDocumentVersion(Document document)
    {
        // Проверка совместимости документа
        return true;
    }

    private void EnsureLibraryLoaded()
    {
        // Загрузка необходимых библиотек
    }

    private void HandleCommandError(Exception ex)
    {
        MessageBox.Show("Ошибка выполнения команды: " + ex.Message);
    }

    private System.Drawing.Icon LoadIcon(string name)
    {
        // Загрузка иконок из ресурсов
        return null;
    }
}
```

### Работа с библиотеками и конфигурациями

```csharp
public class LibraryManager
{
    private LibraryConfigurations _libraries;
    
    public LibraryManager()
    {
        _libraries = new LibraryConfigurations();
    }
    
    public void LoadShaftLibraries()
    {
        // Загрузка стандартных библиотек валов
        string[] standardLibs = {
            "ShaftElements.tws",
            "StandardParts.tws", 
            "Bearings.tws"
        };
        
        foreach (string libName in standardLibs)
        {
            LoadLibraryIfNotExists(libName);
        }
    }
    
    private void LoadLibraryIfNotExists(string libName)
    {
        bool exists = false;
        
        foreach (LibraryConfiguration lib in _libraries)
        {
            if (lib.Name.Contains(libName.Replace(".tws", "")))
            {
                exists = true;
                break;
            }
        }
        
        if (!exists)
        {
            string libPath = Path.Combine(GetLibraryDirectory(), libName);
            if (File.Exists(libPath))
            {
                _libraries.Open(libPath);
            }
        }
    }
    
    public LibraryConfiguration GetActiveShaftLibrary()
    {
        foreach (LibraryConfiguration lib in _libraries)
        {
            if (lib.Name.Contains("Shaft") && lib.IsActive)
            {
                return lib;
            }
        }
        
        // Если нет активной, активировать первую подходящую
        foreach (LibraryConfiguration lib in _libraries)
        {
            if (lib.Name.Contains("Shaft"))
            {
                lib.Activate();
                return lib;
            }
        }
        
        return null;
    }
    
    public void UnloadUnusedLibraries()
    {
        List<LibraryConfiguration> toUnload = new List<LibraryConfiguration>();
        
        foreach (LibraryConfiguration lib in _libraries)
        {
            if (!IsLibraryInUse(lib))
            {
                toUnload.Add(lib);
            }
        }
        
        foreach (LibraryConfiguration lib in toUnload)
        {
            lib.Close();
        }
    }
    
    private bool IsLibraryInUse(LibraryConfiguration lib)
    {
        // Проверка использования библиотеки в текущих документах
        return false; // Заглушка
    }
    
    private string GetLibraryDirectory()
    {
        // Получение пути к директории библиотек
        return Path.Combine(
            Environment.GetFolderPath(Environment.SpecialFolder.ProgramFiles),
            "T-FLEX CAD 17", "Libraries"
        );
    }
}
```

### Создание команд с отменой операций

```csharp
public class UndoableCommand : TFlex.Command
{
    private Document _document;
    private string _operationName;
    private Action _executeAction;
    private Action _undoAction;
    
    public UndoableCommand(Document document, string operationName, 
        Action execute, Action undo)
    {
        _document = document;
        _operationName = operationName;
        _executeAction = execute;
        _undoAction = undo;
    }
    
    public override void Execute()
    {
        _document.BeginChanges(_operationName);
        
        try
        {
            _executeAction();
            _document.EndChanges();
        }
        catch (Exception ex)
        {
            _document.EndChanges();
            throw ex;
        }
    }
    
    public override void Undo()
    {
        _document.BeginChanges("Отмена: " + _operationName);
        
        try
        {
            _undoAction();
            _document.EndChanges();
        }
        catch (Exception ex)
        {
            _document.EndChanges();
            throw ex;
        }
    }
    
    public override string Name => _operationName;
}
```

### Интеграция с системой событий приложения

```csharp
public class EventDrivenPlugin : TFlex.Plugin
{
    public EventDrivenPlugin(Factory factory) : base(factory)
    {
        // Подписка на глобальные события
        TFlex.Application.ApplicationStarted += OnApplicationStarted;
        TFlex.Application.ApplicationClosing += OnApplicationClosing;
    }

    private void OnApplicationStarted(object sender, EventArgs e)
    {
        // Инициализация при запуске приложения
        InitializeGlobalSettings();
        LoadUserPreferences();
    }

    private void OnApplicationClosing(object sender, EventArgs e)
    {
        // Очистка при закрытии приложения
        SaveUserPreferences();
        CleanupResources();
    }

    protected override void DocumentOpenEventHandler(DocumentEventArgs args)
    {
        base.DocumentOpenEventHandler(args);
        
        // Подписка на события документа
        args.Document.ObjectCreated += OnDocumentObjectCreated;
        args.Document.ObjectDeleted += OnDocumentObjectDeleted;
        args.Document.SelectionChanged += OnSelectionChanged;
    }

    private void OnDocumentObjectCreated(object sender, ObjectEventArgs e)
    {
        // Реакция на создание объектов
        if (e.Object.GroupType == ObjectType.Operation)
        {
            OnOperationCreated(e.Object as Operation);
        }
    }

    private void OnDocumentObjectDeleted(object sender, ObjectEventArgs e)
    {
        // Реакция на удаление объектов
        CleanupObjectReferences(e.ObjectId);
    }

    private void OnSelectionChanged(object sender, EventArgs e)
    {
        // Реакция на изменение выделения
        UpdateUIForSelection();
    }

    // Методы обработки событий
    private void OnOperationCreated(Operation operation) { }
    private void CleanupObjectReferences(int objectId) { }
    private void UpdateUIForSelection() { }
    private void InitializeGlobalSettings() { }
    private void LoadUserPreferences() { }
    private void SaveUserPreferences() { }
    private void CleanupResources() { }
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Command_Advanced_Examples.md
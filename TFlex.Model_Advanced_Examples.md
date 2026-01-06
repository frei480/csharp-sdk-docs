# Продвинутые примеры использования классов в пространстве имён TFlex.Model

## Комплексные сценарии работы с документами и объектами

### Управление жизненным циклом документа

```csharp
public void ManageDocumentLifecycle()
{
    Document document = TFlex.Application.ActiveDocument;
    
    // Подписка на события документа
    document.DocumentOpened += OnDocumentOpened;
    document.DocumentClosed += OnDocumentClosed;
    document.ObjectCreated += OnObjectCreated;
    document.ObjectDeleted += OnObjectDeleted;
    
    // Работа с документом
    PerformModelingOperations(document);
    
    // Отписка от событий
    document.DocumentOpened -= OnDocumentOpened;
    document.DocumentClosed -= OnDocumentClosed;
    document.ObjectCreated -= OnObjectCreated;
    document.ObjectDeleted -= OnObjectDeleted;
}

private void OnDocumentOpened(object sender, DocumentEventArgs e)
{
    // Обработка открытия документа
    AttachPluginToDocument(e.Document);
}

private void OnDocumentClosed(object sender, DocumentEventArgs e)
{
    // Обработка закрытия документа
    DetachPluginFromDocument(e.Document);
}
```

### Анализ и фильтрация объектов модели

```csharp
public Dictionary<ObjectType, List<ModelObject>> AnalyzeModelObjects(Document document)
{
    var objectGroups = new Dictionary<ObjectType, List<ModelObject>>();
    
    // Получение всех объектов
    ICollection<ModelObject> allObjects = document.GetObjects();
    
    foreach (ModelObject obj in allObjects)
    {
        ObjectType type = obj.GroupType;
        
        if (!objectGroups.ContainsKey(type))
        {
            objectGroups[type] = new List<ModelObject>();
        }
        
        objectGroups[type].Add(obj);
    }
    
    // Вывод статистики
    foreach (var group in objectGroups)
    {
        Console.WriteLine($"Тип {group.Key}: {group.Value.Count} объектов");
    }
    
    return objectGroups;
}
```

### Работа с фрагментами и внешними ссылками

```csharp
public void ProcessFragments(Document document)
{
    var fragments = new List<Fragment3D>();
    
    // Сбор всех фрагментов
    ICollection<ModelObject> objects = document.GetObjects();
    foreach (ModelObject obj in objects)
    {
        if (obj.GroupType == ObjectType.Fragment)
        {
            Fragment3D fragment = obj as Fragment3D;
            if (fragment != null)
            {
                fragments.Add(fragment);
            }
        }
    }
    
    // Обработка каждого фрагмента
    foreach (Fragment3D fragment in fragments)
    {
        string filePath = fragment.FullFilePath;
        
        if (System.IO.File.Exists(filePath))
        {
            // Открытие документа фрагмента
            Document fragmentDoc = TFlex.Application.OpenDocument(filePath);
            
            // Выполнение операций с фрагментом
            ProcessFragmentDocument(fragmentDoc);
            
            // Сохранение изменений
            fragmentDoc.Save();
            
            // Закрытие документа
            fragmentDoc.Close();
        }
        else
        {
            // Обработка отсутствующего файла
            HandleMissingFragment(fragment);
        }
    }
}
```

### Групповые операции с объектами

```csharp
public void PerformBulkOperations(Document document)
{
    document.BeginChanges("Групповые операции");
    
    try
    {
        // Сбор объектов для обработки
        ObjectArray operations = new ObjectArray();
        ObjectArray lcsObjects = new ObjectArray();
        ObjectArray dimensions = new ObjectArray();
        
        ICollection<ModelObject> allObjects = document.GetObjects();
        foreach (ModelObject obj in allObjects)
        {
            switch (obj.GroupType)
            {
                case ObjectType.Operation:
                    operations.Add(obj);
                    break;
                case ObjectType.LCS:
                    lcsObjects.Add(obj);
                    break;
                case ObjectType.Dimension:
                    dimensions.Add(obj);
                    break;
            }
        }
        
        // Групповое скрытие операций
        foreach (ModelObject op in operations)
        {
            (op as Operation).Visible = false;
        }
        
        // Групповое удаление размеров
        if (dimensions.Count > 0)
        {
            DeleteOptions deleteOptions = new DeleteOptions(true);
            document.DeleteObjects(dimensions, deleteOptions);
        }
        
        document.EndChanges();
    }
    catch (Exception ex)
    {
        document.EndChanges();
        throw ex;
    }
}
```

### Управление выделением объектов

```csharp
public void ManageSelection(Document document)
{
    // Очистка выделения
    document.Selection.Clear();
    
    // Поиск и выделение объектов определенного типа
    ICollection<ModelObject> objects = document.GetObjects();
    foreach (ModelObject obj in objects)
    {
        if (obj.GroupType == ObjectType.Operation && obj.Name.Contains("Shaft"))
        {
            document.Selection.Add(obj);
        }
    }
    
    // Получение количества выделенных объектов
    int selectedCount = document.Selection.Count;
    
    // Обработка выделенных объектов
    for (int i = 0; i < selectedCount; i++)
    {
        ModelObject selectedObj = document.Selection.GetAt(i);
        ProcessSelectedObject(selectedObj);
    }
    
    // Выделение всех объектов определенного типа
    SelectAllObjectsOfType(document, ObjectType.LCS);
}

private void SelectAllObjectsOfType(Document document, ObjectType objectType)
{
    document.Selection.Clear();
    
    ICollection<ModelObject> objects = document.GetObjects();
    foreach (ModelObject obj in objects)
    {
        if (obj.GroupType == objectType)
        {
            document.Selection.Add(obj);
        }
    }
}
```

### Работа с историей изменений документа

```csharp
public void WorkWithDocumentHistory(Document document)
{
    // Проверка возможности отмены
    if (document.CanUndo)
    {
        // Получение имени последней операции
        string lastOperation = document.GetUndoName();
        Console.WriteLine("Последняя операция: " + lastOperation);
        
        // Отмена последней операции
        document.Undo();
    }
    
    // Проверка возможности повтора
    if (document.CanRedo)
    {
        // Получение имени операции для повтора
        string redoOperation = document.GetRedoName();
        Console.WriteLine("Операция для повтора: " + redoOperation);
        
        // Повтор операции
        document.Redo();
    }
    
    // Очистка истории (освобождение памяти)
    document.ClearHistory();
}
```

### Обработка событий объектов модели

```csharp
public void SetupObjectEventHandlers(Document document)
{
    // Подписка на события создания объектов
    document.ObjectCreated += (sender, e) => 
    {
        Console.WriteLine($"Создан объект: {e.Object.Name} типа {e.Object.GroupType}");
        
        // Автоматическая обработка новых объектов
        if (e.Object.GroupType == ObjectType.Operation)
        {
            SetupNewOperation(e.Object as Operation);
        }
    };
    
    // Подписка на события удаления объектов
    document.ObjectDeleted += (sender, e) =>
    {
        Console.WriteLine($"Удален объект: {e.ObjectName} типа {e.ObjectType}");
        
        // Очистка связанных данных
        CleanupObjectData(e.ObjectId);
    };
    
    // Подписка на события изменения объектов
    document.ObjectModified += (sender, e) =>
    {
        Console.WriteLine($"Изменен объект: {e.Object.Name}");
        
        // Обновление зависимых объектов
        UpdateDependentObjects(e.Object);
    };
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model_Advanced_Examples.md
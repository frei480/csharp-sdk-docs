# Примеры использования классов в пространстве имён TFlex.Model

## Описание пространства имён

Пространство имён `TFlex.Model` содержит базовые классы для работы с документами и объектами модели в T-Flex CAD.

## Основные классы

### Document

Класс представляет документ T-Flex CAD, содержащий 3D-модель и 2D-чертежи.

**Пример получения активного документа:**
```csharp
// Получение активного документа
Document document = TFlex.Application.ActiveDocument;

// Проверка наличия документа
if (document == null)
{
    MessageBox.Show("Нет активного документа");
    return;
}
```

**Пример работы с блоками изменений:**
```csharp
// Начало блока изменений
document.BeginChanges("Создание объектов");

// ... операции с моделью ...

// Завершение блока изменений
document.EndChanges();
```

**Пример работы со страницей:**
```csharp
// Получение активной страницы
var activePage = document.ActivePage;

// Границы страницы
double left = activePage.Left.Value;
double right = activePage.Right.Value;
double top = activePage.Top.Value;
double bottom = activePage.Bottom.Value;

// Свойства страницы
double paperWidth = activePage.Properties.Paper.Width;
double paperHeight = activePage.Properties.Paper.Height;
```

### ModelObject

Базовый класс для всех объектов модели (операции, LCS, размеры и т.д.).

**Пример получения объектов документа:**
```csharp
// Получение всех объектов
ICollection<ModelObject> objects = document.GetObjects();

foreach (ModelObject obj in objects)
{
    // Проверка типа объекта
    if (obj.GroupType == ObjectType.Operation)
    {
        Operation operation = obj as Operation;
        // Работа с операцией
    }
}
```

**Пример получения объекта по ID:**
```csharp
// Получение объекта по идентификатору
ModelObject obj = document.GetObjectById(0x30000001);
if (obj != null)
{
    // Работа с объектом
}
```

**Пример получения объекта по имени:**
```csharp
// Получение объекта по имени
ModelObject namedObj = document.GetObjectByName("MyLCS");
if (namedObj != null)
{
    LCS lcs = namedObj as LCS;
    // Работа с LCS
}
```

### Fragment3D

Класс представляет 3D-фрагмент (внешнюю ссылку на модель).

**Пример работы с фрагментом:**
```csharp
// Получение фрагмента из выделения
ModelObject selectedObj = document.Selection.GetAt(0);
Fragment3D fragment = selectedObj as Fragment3D;

if (fragment != null)
{
    // Получение пути к файлу
    string filePath = fragment.FullFilePath;
    
    // Проверка существования файла
    if (!System.IO.File.Exists(filePath))
    {
        MessageBox.Show("Файл фрагмента не найден: " + filePath);
        return;
    }
    
    // Открытие документа фрагмента
    Document fragmentDoc = TFlex.Application.OpenDocument(filePath);
}
```

### ObjectArray

Коллекция объектов модели для групповых операций.

**Пример создания массива для удаления:**
```csharp
ObjectArray objectsToDelete = new ObjectArray();

// Добавление объектов для удаления
objectsToDelete.Add(unusedObject1);
objectsToDelete.Add(unusedObject2);

// Удаление с опциями
DeleteOptions options = new DeleteOptions(true);
document.DeleteObjects(objectsToDelete, options);
```

**Пример сбора объектов определенного типа:**
```csharp
ObjectArray projections = new ObjectArray();

ICollection<ModelObject> allObjects = document.GetObjects();
foreach (ModelObject obj in allObjects)
{
    if (obj.GroupType == ObjectType.Projection)
    {
        projections.Add(obj);
    }
}

// Удаление всех проекций
document.DeleteObjects(projections, new DeleteOptions(true));
```

### ObjectType

Перечисление типов объектов модели.

**Примеры использования:**
```csharp
// Проверка типа объекта
if (obj.GroupType == ObjectType.Operation)
{
    // Это операция
}
else if (obj.GroupType == ObjectType.LCS)
{
    // Это локальная система координат
}
else if (obj.GroupType == ObjectType.Projection)
{
    // Это проекция
}
```

### DeleteOptions

Класс параметров удаления объектов.

**Пример использования:**
```csharp
// Удаление с подтверждением зависимостей
DeleteOptions options = new DeleteOptions(true);
document.DeleteObjects(objectsToDelete, options);

// Удаление без подтверждения
DeleteOptions forceOptions = new DeleteOptions(false);
document.DeleteObjects(objectsToDelete, forceOptions);
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model_Examples.md
# Шпаргалка по классам в пространстве имён TFlex.Model

## Document
| Метод/Свойство | Тип | Описание |
|---|---|---|
| ActivePage | Page | Текущая страница |
| Selection | Selection | Выделенные объекты |
| Properties | DocProperties | Свойства документа |
| BeginChanges(desc) | void | Начало блока изменений |
| EndChanges() | void | Завершение блока |
| GetObjects() | ICollection<ModelObject> | Все объекты |
| GetObjectById(id) | ModelObject | Объект по ID |
| GetObjectByName(name) | ModelObject | Объект по имени |
| DeleteObjects(arr, opt) | void | Удаление объектов |
| Save() | void | Сохранение |
| Close() | void | Закрытие |

## ModelObject
| Свойство | Тип | Описание |
|---|---|---|
| Id | int | Уникальный ID |
| Name | string | Имя объекта |
| GroupType | ObjectType | Тип объекта |
| Visible | bool | Видимость |

## Fragment3D
| Свойство | Тип | Описание |
|---|---|---|
| FullFilePath | string | Полный путь к файлу |
| FileName | string | Имя файла |
| IsLoaded | bool | Загружен ли фрагмент |

## ObjectArray
| Метод | Параметры | Описание |
|---|---|---|
| Add(obj) | ModelObject | Добавление объекта |
| Remove(obj) | ModelObject | Удаление объекта |
| Count | int | Количество |
| GetAt(index) | ModelObject | Объект по индексу |

## ObjectType
- Operation - операция
- LCS - система координат
- Dimension - размер
- Projection - проекция
- Fragment - фрагмент
- Sketch - эскиз
- Variable - переменная
- Parameter - параметр
- Construction - построение

## DeleteOptions
| Конструктор | Описание |
|---|---|
| DeleteOptions(confirm) | confirm - подтверждать зависимости |

## Быстрые примеры

```csharp
// Документ
Document doc = TFlex.Application.ActiveDocument;
doc.BeginChanges("Операция");
try {
    // операции
} finally {
    doc.EndChanges();
}

// Объекты
ICollection<ModelObject> objs = doc.GetObjects();
foreach (ModelObject obj in objs) {
    if (obj.GroupType == ObjectType.Operation) {
        // обработка
    }
}

// Удаление
ObjectArray toDelete = new ObjectArray();
toDelete.Add(obj);
doc.DeleteObjects(toDelete, new DeleteOptions(true));

// Фрагмент
Fragment3D frag = selectedObj as Fragment3D;
string path = frag.FullFilePath;
Document fragDoc = TFlex.Application.OpenDocument(path);
```

## События документа
```csharp
doc.ObjectCreated += (s, e) => Console.WriteLine("Создан: " + e.Object.Name);
doc.ObjectDeleted += (s, e) => Console.WriteLine("Удален: " + e.ObjectName);
doc.DocumentClosed += (s, e) => Cleanup();
```

## Типичные паттерны
```csharp
// Безопасная работа с документом
if (doc == null) return;
doc.BeginChanges("Описание");
try {
    // код
    doc.EndChanges();
} catch {
    doc.EndChanges(); // откат
    throw;
}

// Фильтрация объектов
var operations = doc.GetObjects()
    .Where(o => o.GroupType == ObjectType.Operation)
    .ToList();
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model_Cheat_Sheet.md


Руководство по T-FLEX CAD Open API

# ListItemRole - перечисление  
    
Роль данных элемента ListControl

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public enum ListItemRole
```
```vb
Public Enumeration ListItemRole
```
```cpp
public enum class ListItemRole
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| DefaultRole | 0 | Роль по умолчанию. Ожидается строка, double или int |
| IconRole | 1 | Иконка. Ожидается Icon |
| CheckStateRole | 2 | Состояние чекбокса. Ожидается CheckState |
| CheckIsEnabledRole | 3 | Доступность чекбокса для редактирования. Ожидается bool. |
| CheckIsThreeState | 4 | Чекбокс работает в режиме ThreeState. Ожидается bool. |
| PrecisionRole | 5 | Точность. Ожидается double |
| ToolTipRole | 6 | Всплывающая подсказка. Ожидается строка |
| AlignmentRole | 7 | Выравнивание. Ожидается ListItemAlignment |
| EditableRole | 8 | Поддерживает редактирование. Ожидается bool. |
| ColumnNameRole | 9 | Имя колонки. Если задано, используется при настройке колонок вместо DefaultRole. |
| ColumnIsInitiallyVisibleRole | 10 | Видимость колонки при первом показе. Ожидается bool. |
| ColumnIsGroupRole | 11 | Колонка является группирующей. Ожидается bool. Если задан флаг, колонка будет группирующей по тексту. |
| ColumnIsTreeRole | 12 | Колонка используется для отображения дерева. Ожидается bool. |
| ColumnIsSortableRole | 13 | Колонка поддерживает сортировку. Ожидается bool. Если задан флаг, у колонки будет доступна сортировка. |
| WidthCoefficientRole | 14 | Коэффициент ширины колонки. |
| ColorRole | 15 | Цвет текста. Ожидается System.Drawing.Color |
| BgColorRole | 16 | Цвет фона |
| IdRole | 17 | Роль идентификатор. Ожидается System.Int64 или int |
| ParentIndexRole | 18 | Роль индекс родительского элемента. Ожидается int |
| ParentIdRole | 19 | Роль идентификатор родительского элемента. Ожидается System.Int64 или int |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)
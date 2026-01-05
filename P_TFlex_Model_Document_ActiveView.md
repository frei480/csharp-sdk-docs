

Руководство по T-FLEX CAD Open API

# DocumentActiveView - свойство  
  
---  
  
Объект класса View, представляющий активный (текущий) вид документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public View ActiveView { get; }
```
```vb
Public ReadOnly Property ActiveView As View
	Get
```
```cpp
public:
property View^ ActiveView {
	View^ get ();
}
```


#### Возвращаемое значение

[View](T_TFlex_Model_View.md)Mожет вернуть 0 в том случае если у документа нет активного вида или вообще нет видов.

У документа есть виды только в том случае, если он открыт для редактирования и не является документом фрагмента или временным документом.

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
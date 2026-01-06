

Руководство по T-FLEX CAD Open API

# DocumentAttachPlugin - метод  
    
Подписаться на приход уведомлений о событиях для данного документа.

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void AttachPlugin(
	Plugin plugin
)
```
```vb
Public Sub AttachPlugin ( 
	plugin As Plugin
)
```
```cpp
public:
void AttachPlugin(
	Plugin^ plugin
)
```


#### Параметры

plugin [Plugin](T_TFlex_Plugin.md)
    Объект класса приложения

Использование данного метода касается всех уведомлений, которые связаны с конкретным документом, а именно: 

  * [SavingDocumentEventHandler(DocumentEventArgs)](M_TFlex_Plugin_SavingDocumentEventHandler.md) \- вызывается перед сохранением документа
  * [DocumentSavedEventHandler(DocumentEventArgs)](M_TFlex_Plugin_DocumentSavedEventHandler.md) \- вызывается после успешного сохранения документа
  * [ClosingDocumentEventHandler(DocumentEventArgs)](M_TFlex_Plugin_ClosingDocumentEventHandler.md) \- вызывается перед закрытием документа
  * [ViewActivatedEventHandler(ViewEventArgs)](M_TFlex_Plugin_ViewActivatedEventHandler.md) \- вызывается после активизации окна документа
  * [ViewDeactivatedEventHandler(ViewEventArgs)](M_TFlex_Plugin_ViewDeactivatedEventHandler.md) \- вызывается после деактивизации окна документа 
  * [DynamicAnalysisSteppedEventHandler(DynamicAnalysisEventArgs)](M_TFlex_Plugin_DynamicAnalysisSteppedEventHandler.md) \- вызывается при выполнении различных задач динамического анализа
  * [ObjectCreatedEventHandler(ObjectEventArgs)](M_TFlex_Plugin_ObjectCreatedEventHandler.md) \- вызывается после создания объекта
  * [DeletingObjectEventHandler(ObjectEventArgs)](M_TFlex_Plugin_DeletingObjectEventHandler.md) \- вызывается перед удалением объекта
  * [ObjectDeletedEventHandler(ObjectEventArgs)](M_TFlex_Plugin_ObjectDeletedEventHandler.md) \- вызывается после удаления объекта
  * [ObjectChangedEventHandler(ObjectEventArgs)](M_TFlex_Plugin_ObjectChangedEventHandler.md) \- вызывается после изменения объекта
  * [ObjectSelectionChangedEventHandler(ObjectEventArgs)](M_TFlex_Plugin_ObjectSelectionChangedEventHandler.md) \- вызывается при изменении селекции объекта
  * [RegeneratingDocumentEventHandler(RegenerateDocumentEventArgs)](M_TFlex_Plugin_RegeneratingDocumentEventHandler.md) \- вызывается перед пересчётом документа
  * [DocumentRegeneratedEventHandler(RegenerateDocumentEventArgs)](M_TFlex_Plugin_DocumentRegeneratedEventHandler.md) \- вызывается после пересчёта документа
  * [TrackingContextPopupMenuEventHandler(TrackingContextPopupMenuEventArgs)](M_TFlex_Plugin_TrackingContextPopupMenuEventHandler.md) \- вызывается перед показом контекстного меню объекта
  * [DrawingDocumentEventHandler(DrawingDocumentEventArgs)](M_TFlex_Plugin_DrawingDocumentEventHandler.md) \- вызывается перед отрисовкой документа
  * [DocumentDrawnEventHandler(DrawingDocumentEventArgs)](M_TFlex_Plugin_DocumentDrawnEventHandler.md) \- вызывается после отрисовки документа



#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)


Руководство по T-FLEX CAD Open API

# DocumentBeginChanges - метод  
  
---  
  
Открытие блока изменения документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void BeginChanges(
	string name
)
```
```vb
Public Sub BeginChanges ( 
	name As String
)
```
```cpp
public:
void BeginChanges(
	String^ name
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Задаёт имя блока изменения документа

Для выполнения любых изменений в документе (создание новых объектов, удаление объектов, изменение объектов) необходимо открыть блок действий по изменению документа (блок изменения документа) Одновременно может быть открыт только один блок изменения документа. Вложение блоков изменения документа не допускается. Для закрытия блока изменения документа необходимо вызвать [EndChanges](M_TFlex_Model_Document_EndChanges.md) или [CancelChanges](M_TFlex_Model_Document_CancelChanges.md). Имя блока изменения документа отображается в диалоге отмены и повтора действий.

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
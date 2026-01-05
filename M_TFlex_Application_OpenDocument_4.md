

Руководство по T-FLEX CAD Open API

# ApplicationOpenDocument(FileLink) - метод  
  
---  
  
Открыть документ

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Document OpenDocument(
	FileLink link
)
```
```vb
Public Shared Function OpenDocument ( 
	link As FileLink
) As Document
```
```cpp
public:
static Document^ OpenDocument(
	FileLink^ link
)
```


#### Параметры

link [FileLink](T_TFlex_Model_FileLink.md)
    Ссылка на файл документа

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Открытый документ или null в случае ошибки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[OpenDocument - перегрузка](Overload_TFlex_Application_OpenDocument.md)

[TFlex - пространство имён](N_TFlex.md)
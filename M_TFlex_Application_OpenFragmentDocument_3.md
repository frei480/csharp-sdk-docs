

Руководство по T-FLEX CAD Open API

# ApplicationOpenFragmentDocument(FileLink, Boolean, Boolean) - метод  
  
---  
  
Открыть документ фрагмента для чтения

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Document OpenFragmentDocument(
	FileLink link,
	bool with3D,
	bool recalculate
)
```
```vb
Public Shared Function OpenFragmentDocument ( 
	link As FileLink,
	with3D As Boolean,
	recalculate As Boolean
) As Document
```
```cpp
public:
static Document^ OpenFragmentDocument(
	FileLink^ link, 
	bool with3D, 
	bool recalculate
)
```


#### Параметры

link [FileLink](T_TFlex_Model_FileLink.md)
    Ссылка на файл документа
with3D [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
recalculate [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Открытый документ или null в случае ошибки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[OpenFragmentDocument - перегрузка](Overload_TFlex_Application_OpenFragmentDocument.md)

[TFlex - пространство имён](N_TFlex.md)
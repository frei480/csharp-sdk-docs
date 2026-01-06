

Руководство по T-FLEX CAD Open API

# ApplicationNewDocument(Boolean) - метод  
    
Создать новый документ

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Document NewDocument(
	bool b3D
)
```
```vb
Public Shared Function NewDocument ( 
	b3D As Boolean
) As Document
```
```cpp
public:
static Document^ NewDocument(
	bool b3D
)
```


#### Параметры

b3D [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    В случае, если параметр равен true, новый документ создаётся на основе 3D прототипа

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Созданный документ или null в случае ошибки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[NewDocument - перегрузка](Overload_TFlex_Application_NewDocument.md)

[TFlex - пространство имён](N_TFlex.md)
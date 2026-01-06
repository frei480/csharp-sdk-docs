

Руководство по T-FLEX CAD Open API

# ModelObjectSetFileLinkReference(Int32, FileLink, ModelObjectArrayIndices) - метод  
    
Установить ссылку на файл по ключу и индексу. Используется для организации массивов

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetFileLinkReference(
	int id,
	FileLink link,
	ModelObjectArrayIndices indices
)
```
```vb
Public Sub SetFileLinkReference ( 
	id As Integer,
	link As FileLink,
	indices As ModelObjectArrayIndices
)
```
```cpp
public:
void SetFileLinkReference(
	int id, 
	FileLink^ link, 
	ModelObjectArrayIndices^ indices
)
```


#### Параметры

id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор ключа, по которому в контейнере ссылок хранится ссылка
link [FileLink](T_TFlex_Model_FileLink.md)
    Ссылка на файл
indices [ModelObjectArrayIndices](T_TFlex_Model_ModelObject_ArrayIndices.md)
    Координаты элемента

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[SetFileLinkReference - перегрузка](Overload_TFlex_Model_ModelObject_SetFileLinkReference.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
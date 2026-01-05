

Руководство по T-FLEX CAD Open API

# InternalDatabaseInsertTextColumn - метод  
  
---  
  
Вставить текстовый столбец с указанием длины текста

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int InsertTextColumn(
	int index,
	string name,
	int length
)
```
```vb
Public Function InsertTextColumn ( 
	index As Integer,
	name As String,
	length As Integer
) As Integer
```
```cpp
public:
int InsertTextColumn(
	int index, 
	String^ name, 
	int length
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер столбца
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Название столбца
length [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Количество символов

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

#### Ссылки

[InternalDatabase - ](T_TFlex_Model_InternalDatabase.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
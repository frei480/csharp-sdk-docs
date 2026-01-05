

Руководство по T-FLEX CAD Open API

# LeaderNoteGetLeaderDOCsLinks - метод  
  
---  
  
Получение позиций полках надписи

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public List<Guid> GetLeaderDOCsLinks(
	int StringIndex
)
```
```vb
Public Function GetLeaderDOCsLinks ( 
	StringIndex As Integer
) As List(Of Guid)
```
```cpp
public:
List<Guid>^ GetLeaderDOCsLinks(
	int StringIndex
)
```


#### Параметры

StringIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс дополнительной полки (начиная с 0). "-1" для основной полки.

#### Возвращаемое значение

[List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[Guid](https://learn.microsoft.com/dotnet/api/system.guid)Список позиций

#### Ссылки

[LeaderNote - ](T_TFlex_Model_Model2D_LeaderNote.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
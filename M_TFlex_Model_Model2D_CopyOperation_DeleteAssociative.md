

Руководство по T-FLEX CAD Open API

# CopyOperationDeleteAssociative - метод  
    
Удаление ассоциативного объекта

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool DeleteAssociative(
	int indexSource,
	int indexTransformation
)
```
```vb
Public Function DeleteAssociative ( 
	indexSource As Integer,
	indexTransformation As Integer
) As Boolean
```
```cpp
public:
bool DeleteAssociative(
	int indexSource, 
	int indexTransformation
)
```


#### Параметры

indexSource [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс исходного объекта в списке объекта-копии
indexTransformation [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс преобразования

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)false - если индексы выходит за границы списка исходных объектов и трансформаций

#### Ссылки

[CopyOperation - ](T_TFlex_Model_Model2D_CopyOperation.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
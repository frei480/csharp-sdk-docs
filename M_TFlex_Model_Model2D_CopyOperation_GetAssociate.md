

Руководство по T-FLEX CAD Open API

# CopyOperationGetAssociate - метод  
    
Получение ассоциативного объекта (результата копирования)

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Object2D GetAssociate(
	int indexSource,
	int indexTransformation
)
```
```vb
Public Function GetAssociate ( 
	indexSource As Integer,
	indexTransformation As Integer
) As Object2D
```
```cpp
public:
Object2D^ GetAssociate(
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

[Object2D](T_TFlex_Model_Model2D_Object2D.md)Ассоциативный объект (результат копирования)

#### Ссылки

[CopyOperation - ](T_TFlex_Model_Model2D_CopyOperation.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
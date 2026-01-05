

Руководство по T-FLEX CAD Open API

# DynamicStudyGetRestraint - метод  
  
---  
  
Получить нагружение по номеру

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Restraint GetRestraint(
	int index
)
```
```vb
Public Function GetRestraint ( 
	index As Integer
) As Restraint
```
```cpp
public:
Restraint^ GetRestraint(
	int index
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер нагружения

#### Возвращаемое значение

[Restraint](T_TFlex_Model_Model3D_Restraint.md)

Элементы нумеруются от нуля. Если индекс отрицательный или превышает количество элементов, то результат не определён

#### Ссылки

[DynamicStudy - ](T_TFlex_Model_Model3D_DynamicStudy.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
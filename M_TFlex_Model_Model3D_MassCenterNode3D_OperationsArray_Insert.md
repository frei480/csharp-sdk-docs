

Руководство по T-FLEX CAD Open API

# MassCenterNode3DOperationsArrayInsert - метод  
    
Вставить операцию перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int index,
	Operation operation
)
```




#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер операции
operation [Operation](T_TFlex_Model_Model3D_Operation.md)
    Вставляемая операция

Операции нумеруются от нуля. Если индекс отрицательный или превышает количество операций, то результат не определён

#### Ссылки

[MassCenterNode3DOperationsArray - ](T_TFlex_Model_Model3D_MassCenterNode3D_OperationsArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
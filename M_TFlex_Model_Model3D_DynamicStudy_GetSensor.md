

Руководство по T-FLEX CAD Open API

# DynamicStudyGetSensor - метод  
    
Получить датчик по номеру

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Sensor GetSensor(
	int index
)
```
```vb
Public Function GetSensor ( 
	index As Integer
) As Sensor
```
```cpp
public:
Sensor^ GetSensor(
	int index
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер датчика

#### Возвращаемое значение

[Sensor](T_TFlex_Model_Model3D_Sensor.md)

Элементы нумеруются от нуля. Если индекс отрицательный или превышает количество элементов, то результат неопределён

#### Ссылки

[DynamicStudy - ](T_TFlex_Model_Model3D_DynamicStudy.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
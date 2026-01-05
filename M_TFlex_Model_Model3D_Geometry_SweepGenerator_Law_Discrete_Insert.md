

Руководство по T-FLEX CAD Open API

# SweepGeneratorLawDiscreteInsert - метод  
  
---  
  
Вставить пару перед номером

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	uint index,
	SweepGeneratorLawDiscreteAssociation pair
)
```
```vb
Public Sub Insert ( 
	index As UInteger,
	pair As SweepGeneratorLawDiscreteAssociation
)
```
```cpp
public:
void Insert(
	unsigned int index, 
	SweepGeneratorLawDiscreteAssociation^ pair
)
```


#### Параметры

index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер пары
pair [SweepGeneratorLawDiscreteAssociation](T_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete_Association.md)
    

Пары нумеруются от нуля. Если индекс отрицательный или превышает количество пар, то результат не определён

#### Ссылки

[SweepGeneratorLawDiscrete - ](T_TFlex_Model_Model3D_Geometry_SweepGenerator_Law_Discrete.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
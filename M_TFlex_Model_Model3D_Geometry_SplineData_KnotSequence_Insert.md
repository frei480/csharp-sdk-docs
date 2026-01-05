

Руководство по T-FLEX CAD Open API

# SplineDataKnotSequenceInsert - метод  
  
---  
  
Вставить узел перед номером

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	uint Index,
	SplineDataKnotSequenceKnot knot
)
```
```vb
Public Sub Insert ( 
	Index As UInteger,
	knot As SplineDataKnotSequenceKnot
)
```
```cpp
public:
void Insert(
	unsigned int Index, 
	SplineDataKnotSequenceKnot^ knot
)
```


#### Параметры

Index [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер узла, перед которым будет вставлен данный узел
knot [SplineDataKnotSequenceKnot](T_TFlex_Model_Model3D_Geometry_SplineData_KnotSequence_Knot.md)
    Узел

Узлы нумеруются от нуля. Если индекс отрицательный или превышает количество узлов, то результат неопределён

#### Ссылки

[SplineDataKnotSequence - ](T_TFlex_Model_Model3D_Geometry_SplineData_KnotSequence.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
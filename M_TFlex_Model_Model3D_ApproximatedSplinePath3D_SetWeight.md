

Руководство по T-FLEX CAD Open API

# ApproximatedSplinePath3DSetWeight - метод  
    
Установить вес точки

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetWeight(
	int index,
	Parameter weight
)
```
```vb
Public Sub SetWeight ( 
	index As Integer,
	weight As Parameter
)
```
```cpp
public:
void SetWeight(
	int index, 
	Parameter^ weight
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки
weight [Parameter](T_TFlex_Model_Parameter.md)
    Вес точки

Вес должен быть больше нуля

#### Ссылки

[ApproximatedSplinePath3D - ](T_TFlex_Model_Model3D_ApproximatedSplinePath3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# LoftRemoveCoupling - метод  
    
Удалить последовательность точек соответсвия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void RemoveCoupling(
	int couplingIndex
)
```
```vb
Public Sub RemoveCoupling ( 
	couplingIndex As Integer
)
```
```cpp
public:
void RemoveCoupling(
	int couplingIndex
)
```


#### Параметры

couplingIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс последовательности точек соответствия

Для 0-го соответствия (couplingIndex=0) эта операция интерпретируется как удаление стартовых точек соответствия (они заменяются на стартовые точки по умолчанию), само соответствие не удаляется

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

RemoveCoupling(Int32)

[ResetCouplingPoint(Int32, Int32)](M_TFlex_Model_Model3D_Loft_ResetCouplingPoint.md)
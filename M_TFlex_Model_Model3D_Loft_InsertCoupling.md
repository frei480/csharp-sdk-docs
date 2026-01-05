

Руководство по T-FLEX CAD Open API

# LoftInsertCoupling - метод  
  
---  
  
Вставить последовательность точек соответсвия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void InsertCoupling(
	int couplingIndex
)
```
```vb
Public Sub InsertCoupling ( 
	couplingIndex As Integer
)
```
```cpp
public:
void InsertCoupling(
	int couplingIndex
)
```


#### Параметры

couplingIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс последовательности точек соответствия

Последовательность точек соответствия проходит через все невырожденные профили. Всегда существует последовательность точек соответствия с нулевым индексом, включающая стартовые точки по умолчанию со всех невырожденных профилей.

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[RemoveCoupling(Int32)](M_TFlex_Model_Model3D_Loft_RemoveCoupling.md)

[SetCouplingPoint(Int32, Int32, LoftPointOnContour)](M_TFlex_Model_Model3D_Loft_SetCouplingPoint.md)
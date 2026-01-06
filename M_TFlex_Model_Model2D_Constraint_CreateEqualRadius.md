

Руководство по T-FLEX CAD Open API

# ConstraintCreateEqualRadius - метод  
    
Создать ограничение "Равный радиус" 

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Constraint CreateEqualRadius(
	Document iDoc,
	Object2D iObject1,
	Object2D iObject2
)
```
```vb
Public Shared Function CreateEqualRadius ( 
	iDoc As Document,
	iObject1 As Object2D,
	iObject2 As Object2D
) As Constraint
```
```cpp
public:
static Constraint^ CreateEqualRadius(
	Document^ iDoc, 
	Object2D^ iObject1, 
	Object2D^ iObject2
)
```


#### Параметры

iDoc [Document](T_TFlex_Model_Document.md)
     Текущий документ 
iObject1 [Object2D](T_TFlex_Model_Model2D_Object2D.md)
     Первый опорный объект 
iObject2 [Object2D](T_TFlex_Model_Model2D_Object2D.md)
     Второй опорный объект 

#### Возвращаемое значение

[Constraint](T_TFlex_Model_Model2D_Constraint.md) Объект "Ограничение" - в случае успеха 

#### Ссылки

[Constraint - ](T_TFlex_Model_Model2D_Constraint.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
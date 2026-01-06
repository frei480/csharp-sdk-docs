

Руководство по T-FLEX CAD Open API

# ConstraintCreateMidPoint - метод  
    
Создать ограничение "Симметрия" 

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Constraint CreateMidPoint(
	Document iDoc,
	Object2D iObject1,
	ConstraintPointType iPoint1,
	Object2D iObject2,
	ConstraintPointType iPoint2,
	Object2D iObject3,
	ConstraintPointType iPoint3
)
```
```vb
Public Shared Function CreateMidPoint ( 
	iDoc As Document,
	iObject1 As Object2D,
	iPoint1 As ConstraintPointType,
	iObject2 As Object2D,
	iPoint2 As ConstraintPointType,
	iObject3 As Object2D,
	iPoint3 As ConstraintPointType
) As Constraint
```
```cpp
public:
static Constraint^ CreateMidPoint(
	Document^ iDoc, 
	Object2D^ iObject1, 
	ConstraintPointType iPoint1, 
	Object2D^ iObject2, 
	ConstraintPointType iPoint2, 
	Object2D^ iObject3, 
	ConstraintPointType iPoint3
)
```


#### Параметры

iDoc [Document](T_TFlex_Model_Document.md)
     Текущий документ 
iObject1 [Object2D](T_TFlex_Model_Model2D_Object2D.md)
     Первый опорный объект 
iPoint1 [ConstraintPointType](T_TFlex_Model_Model2D_ConstraintPointType.md)
     Характерная точка первого опорного объекта 
iObject2 [Object2D](T_TFlex_Model_Model2D_Object2D.md)
     Второй опорный объект 
iPoint2 [ConstraintPointType](T_TFlex_Model_Model2D_ConstraintPointType.md)
     Характерная точка второго опорного объекта 
iObject3 [Object2D](T_TFlex_Model_Model2D_Object2D.md)
     Опорный объект, задающий центр для первого и второго опорных объектов 
iPoint3 [ConstraintPointType](T_TFlex_Model_Model2D_ConstraintPointType.md)
     Характерная точка третьего опорного объекта 

#### Возвращаемое значение

[Constraint](T_TFlex_Model_Model2D_Constraint.md) Объект "Ограничение" - в случае успеха 

#### Ссылки

[Constraint - ](T_TFlex_Model_Model2D_Constraint.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# ConstraintCreateFixedLength - метод  
    
Создать ограничение "Фиксированная длина" 

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Constraint CreateFixedLength(
	Document iDoc,
	Object2D iObject
)
```
```vb
Public Shared Function CreateFixedLength ( 
	iDoc As Document,
	iObject As Object2D
) As Constraint
```
```cpp
public:
static Constraint^ CreateFixedLength(
	Document^ iDoc, 
	Object2D^ iObject
)
```


#### Параметры

iDoc [Document](T_TFlex_Model_Document.md)
     Текущий документ 
iObject [Object2D](T_TFlex_Model_Model2D_Object2D.md)
     Опорный объект 

#### Возвращаемое значение

[Constraint](T_TFlex_Model_Model2D_Constraint.md) Объект "Ограничение" - в случае успеха 

#### Ссылки

[Constraint - ](T_TFlex_Model_Model2D_Constraint.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
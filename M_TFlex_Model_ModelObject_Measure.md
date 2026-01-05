

Руководство по T-FLEX CAD Open API

# ModelObjectMeasure(ObjectArray, String, ModelObject) - метод  
  
---  
  
Измерить параметр одного объекта либо отношение нескольких объектов

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Value Measure(
	ObjectArray objects,
	string valueName,
	ModelObject lcs
)
```
```vb
Public Shared Function Measure ( 
	objects As ObjectArray,
	valueName As String,
	lcs As ModelObject
) As Value
```
```cpp
public:
static Value^ Measure(
	ObjectArray^ objects, 
	String^ valueName, 
	ModelObject^ lcs
)
```


#### Параметры

objects [ObjectArray](T_TFlex_Model_ObjectArray.md)
    Измеряемые объекты
valueName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя параметра для измерения, например Distance (см. команду Измерить в пользовательском интерфейсе)
lcs [ModelObject](T_TFlex_Model_ModelObject.md)
    Система координат

#### Возвращаемое значение

[Value](T_TFlex_Model_Measure_Value.md)

#### Ссылки

[ModelObject - ](T_TFlex_Model_ModelObject.md)

[Measure - перегрузка](Overload_TFlex_Model_ModelObject_Measure.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
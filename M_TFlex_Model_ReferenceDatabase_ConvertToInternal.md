

Руководство по T-FLEX CAD Open API

# ReferenceDatabaseConvertToInternal - метод  
  
---  
  
Конвертировать базу данных во внутреннюю базу данных

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static InternalDatabase ConvertToInternal(
	ReferenceDatabase sourceDatabase
)
```
```vb
Public Shared Function ConvertToInternal ( 
	sourceDatabase As ReferenceDatabase
) As InternalDatabase
```
```cpp
public:
static InternalDatabase^ ConvertToInternal(
	ReferenceDatabase^ sourceDatabase
)
```


#### Параметры

sourceDatabase [ReferenceDatabase](T_TFlex_Model_ReferenceDatabase.md)
    База данных по ссылке

#### Возвращаемое значение

[InternalDatabase](T_TFlex_Model_InternalDatabase.md)Внутренняя база данных

При конвертации исходный объект разрушается

#### Ссылки

[ReferenceDatabase - ](T_TFlex_Model_ReferenceDatabase.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
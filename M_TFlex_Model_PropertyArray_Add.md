

Руководство по T-FLEX CAD Open API

# PropertyArrayAdd(String, String, PropertyArrayType) - метод  
    
Добавить свойство в массив свойств

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int Add(
	string Name,
	string Description,
	PropertyArrayType TypeID
)
```
```vb
Public Function Add ( 
	Name As String,
	Description As String,
	TypeID As PropertyArrayType
) As Integer
```
```cpp
public:
int Add(
	String^ Name, 
	String^ Description, 
	PropertyArrayType TypeID
)
```


#### Параметры

Name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя свойства
Description [String](https://learn.microsoft.com/dotnet/api/system.string)
    Описание свойства
TypeID [PropertyArrayType](T_TFlex_Model_PropertyArray_Type.md)
    ID типа свойства

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

#### Ссылки

[PropertyArray - ](T_TFlex_Model_PropertyArray.md)

[Add - перегрузка](Overload_TFlex_Model_PropertyArray_Add.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)


Руководство по T-FLEX CAD Open API

# DocumentGetObjectByName - метод  
    
Получение объекта по имени

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ModelObject GetObjectByName(
	string name
)
```
```vb
Public Function GetObjectByName ( 
	name As String
) As ModelObject
```
```cpp
public:
ModelObject^ GetObjectByName(
	String^ name
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя объекта

#### Возвращаемое значение

[ModelObject](T_TFlex_Model_ModelObject.md)Найденный объект или null если объект не найден

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
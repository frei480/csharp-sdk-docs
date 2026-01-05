

Руководство по T-FLEX CAD Open API

# HoleGetVariableValue - метод  
  
---  
  
Получить переменную отверстия по имени

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FragmentVariableValue GetVariableValue(
	int hole,
	string name,
	bool forSet
)
```
```vb
Public Function GetVariableValue ( 
	hole As Integer,
	name As String,
	forSet As Boolean
) As FragmentVariableValue
```
```cpp
public:
FragmentVariableValue^ GetVariableValue(
	int hole, 
	String^ name, 
	bool forSet
)
```


#### Параметры

hole [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс отверстия
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя переменной отверстия
forSet [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак необходимости изменения переменной

#### Возвращаемое значение

[FragmentVariableValue](T_TFlex_Model_FragmentVariableValue.md)Переменная отверстия

#### Ссылки

[Hole - ](T_TFlex_Model_Model3D_Hole.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
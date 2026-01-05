

Руководство по T-FLEX CAD Open API

# Fragment3DGetVariableValue(String, Boolean, Boolean) - метод  
  
---  
  
Получить переменную фрагмента по имени

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public FragmentVariableValue GetVariableValue(
	string name,
	bool forSet,
	bool onlyExternal
)
```
```vb
Public Function GetVariableValue ( 
	name As String,
	forSet As Boolean,
	onlyExternal As Boolean
) As FragmentVariableValue
```
```cpp
public:
FragmentVariableValue^ GetVariableValue(
	String^ name, 
	bool forSet, 
	bool onlyExternal
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя переменной
forSet [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак необходимости изменения переменной
onlyExternal [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    

#### Возвращаемое значение

[FragmentVariableValue](T_TFlex_Model_FragmentVariableValue.md)Переменная фрагмента

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[GetVariableValue - перегрузка](Overload_TFlex_Model_Model3D_Fragment3D_GetVariableValue.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
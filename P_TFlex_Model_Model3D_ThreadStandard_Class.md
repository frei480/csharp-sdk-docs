

Руководство по T-FLEX CAD Open API

# ThreadStandardClass - свойство  
    
Получить класс точности

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ThreadClass this[
	ThreadSide side,
	int index
] { get; }
```
```vb
Public ReadOnly Property Class ( 
	side As ThreadSide,
	index As Integer
) As ThreadClass
	Get
```
```cpp
public:
property ThreadClass Class[ThreadSide side, int index] {
	ThreadClass get (ThreadSide side, int index);
}
```


#### Параметры

side [ThreadSide](T_TFlex_Model_Model3D_ThreadSide.md)
    
index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Значение свойства

[ThreadClass](T_TFlex_Model_Model3D_ThreadClass.md)

#### Ссылки

[ThreadStandard - ](T_TFlex_Model_Model3D_ThreadStandard.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
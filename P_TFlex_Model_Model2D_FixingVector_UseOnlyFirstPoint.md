

Руководство по T-FLEX CAD Open API

# FixingVectorUseOnlyFirstPoint - свойство  
    
Использовать только первую точку

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public bool UseOnlyFirstPoint { get; set; }
```
```vb
Public Property UseOnlyFirstPoint As Boolean
	Get
	Set
```
```cpp
public:
property bool UseOnlyFirstPoint {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

При установке данного свойства в true, второй узел удаляется. При установки данного свойства в false, после вызова данного свойства необходимо заново задать второй узел с помощью свойства [EndNode](P_TFlex_Model_Model2D_FixingVector_EndNode.md)

#### Ссылки

[FixingVector - ](T_TFlex_Model_Model2D_FixingVector.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
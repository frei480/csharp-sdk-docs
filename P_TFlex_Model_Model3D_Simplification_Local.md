

Руководство по T-FLEX CAD Open API

# SimplificationLocal - свойство  
  
---  
  
Упрощять геометрию отдельно для каждого элемента

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool Local { get; set; }
```
```vb
Public Property Local As Boolean
	Get
	Set
```
```cpp
public:
property bool Local {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Имеет смысл, если список упрощаемых граней пустой, то есть упрощение геометрии выполняется на всех гранях. Имеет смысл, если включен режим упрощения геометрии.

#### Ссылки

[Simplification - ](T_TFlex_Model_Model3D_Simplification.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# SweptSynchronize - свойство  
  
---  
  
Синхронизация начала пути с положением контура

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool Synchronize { get; set; }
```
```vb
Public Property Synchronize As Boolean
	Get
	Set
```
```cpp
public:
property bool Synchronize {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Это свойство актуально для замкнутых путей, когда стартовая точка актуальна для получения правильного пути

#### Ссылки

[Swept - ](T_TFlex_Model_Model3D_Swept.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
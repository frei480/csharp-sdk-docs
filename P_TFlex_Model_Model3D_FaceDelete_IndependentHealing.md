

Руководство по T-FLEX CAD Open API

# FaceDeleteIndependentHealing - свойство  
  
---  
  
Независимая обработка циклов

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool IndependentHealing { get; set; }
```
```vb
Public Property IndependentHealing As Boolean
	Get
	Set
```
```cpp
public:
property bool IndependentHealing {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Если установлено в true, то каждый замкнутый цикл образуемый гранями обрабатывается независимо. В противном случае обрабатываются совместно.

#### Ссылки

[FaceDelete - ](T_TFlex_Model_Model3D_FaceDelete.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
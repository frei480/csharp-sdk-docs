

Руководство по T-FLEX CAD Open API

# LoftThinWall - свойство  
  
---  
  
Тонкостенное построение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool ThinWall { get; set; }
```
```vb
Public Property ThinWall As Boolean
	Get
	Set
```
```cpp
public:
property bool ThinWall {
	bool get ();
	void set (bool value);
}
```


#### Значение свойства

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Если в качестве первого и/или последнего профиля выбрано листовое тело, то данная опция позволяет построить Лофтинг без граней соответствующих первому и последнему профилю, используя только их контуры. Данная опция не может быть использована, если задано периодическое построение

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[Periodic](P_TFlex_Model_Model3D_Loft_Periodic.md)
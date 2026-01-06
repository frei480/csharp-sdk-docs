

Руководство по T-FLEX CAD Open API

# LoftLastEndProfileCondition - свойство  
    
Специальное граничное условие для последнего профиля, condition может быть равно 0

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public LoftEndProfileCondition LastEndProfileCondition { get; set; }
```
```vb
Public Property LastEndProfileCondition As LoftEndProfileCondition
	Get
	Set
```
```cpp
public:
property LoftEndProfileCondition^ LastEndProfileCondition {
	LoftEndProfileCondition^ get ();
	void set (LoftEndProfileCondition^ value);
}
```


#### Значение свойства

[LoftEndProfileCondition](T_TFlex_Model_Model3D_Loft_EndProfileCondition.md)

Граниное условие для профиля может быть установлено, если: Не задан первый вырожденный профиль. Для профиля не задано векторное условие или условие касания с гранью. Лофт не является периодическим.

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
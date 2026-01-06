

Руководство по T-FLEX CAD Open API

# DraggerManagerAddDragger - метод  
    
Регистрирует манипулятор

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public int AddDragger(
	Dragger dragger
)
```




#### Параметры

dragger [Dragger](T_TFlex_Model_Model3D_Visual_Dragger.md)
    

#### Возвращаемое значение

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)Идентификатор, который может быть использован в методах GetDragger и RemoveDragger

Только после вызова этого метода манипулятор изображается в 3D окне и может выбираться. Манипулятор может быть зарегистрирован только один раз в одном диспетчере. 

#### Ссылки

[DraggerManager - ](T_TFlex_Model_Model3D_Visual_DraggerManager.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)
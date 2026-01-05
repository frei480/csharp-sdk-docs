

Руководство по T-FLEX CAD Open API

# BaseBodyClashBody - метод  
  
---  
  
**Примечание: Данный API устарел.**

Функция определяет перекрытие тел

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This method is obsolete, value will not be returned and will be removed. Please use 'Clash' method.")]
public BaseBodyTypeOfClashing ClashBody(
	BaseBody body
)
```
```vb
<ObsoleteAttribute("This method is obsolete, value will not be returned and will be removed. Please use 'Clash' method.")>
Public Function ClashBody ( 
	body As BaseBody
) As BaseBodyTypeOfClashing
```
```cpp
public:
[ObsoleteAttribute(L"This method is obsolete, value will not be returned and will be removed. Please use 'Clash' method.")]
BaseBodyTypeOfClashing ClashBody(
	BaseBody^ body
)
```


#### Параметры

body [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)
    Тело для проверки

#### Возвращаемое значение

[BaseBodyTypeOfClashing](T_TFlex_Model_Model3D_Geometry_BaseBody_TypeOfClashing.md)Тип пересечения

#### Ссылки

[BaseBody - ](T_TFlex_Model_Model3D_Geometry_BaseBody.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
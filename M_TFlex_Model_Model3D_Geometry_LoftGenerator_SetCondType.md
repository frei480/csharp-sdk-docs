

Руководство по T-FLEX CAD Open API

# LoftGeneratorSetCondType - метод  
  
---  
  
Функция задаёт граничное условие в начале-конце лофтинга

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetCondType(
	TFBoundCondType t,
	bool isFirst,
	BaseBody sheet
)
```
```vb
Public Sub SetCondType ( 
	t As TFBoundCondType,
	isFirst As Boolean,
	sheet As BaseBody
)
```
```cpp
public:
void SetCondType(
	TFBoundCondType t, 
	bool isFirst, 
	BaseBody^ sheet
)
```


#### Параметры

t [TFBoundCondType](T_TFlex_Model_Model3D_Geometry_TFBoundCondType.md)
    Тип граничного условия
isFirst [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Параметр отвечающий за то для какого профиля (первого или последнего) задано условие
sheet [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)
    Тело с которого берётся граничное условие

#### Ссылки

[LoftGenerator - ](T_TFlex_Model_Model3D_Geometry_LoftGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
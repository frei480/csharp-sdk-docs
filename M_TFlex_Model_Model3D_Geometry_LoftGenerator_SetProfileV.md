

Руководство по T-FLEX CAD Open API

# LoftGeneratorSetProfileV - метод  
    
Функция задаёт профиль в направлении V

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetProfileV(
	BaseBody prf,
	int num,
	bool orient
)
```
```vb
Public Sub SetProfileV ( 
	prf As BaseBody,
	num As Integer,
	orient As Boolean
)
```
```cpp
public:
void SetProfileV(
	BaseBody^ prf, 
	int num, 
	bool orient
)
```


#### Параметры

prf [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)
    Тело профиля (листовое тело или проволока)
num [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер профиля в списке
orient [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Ориентация с которой профиль входит в генератор

#### Ссылки

[LoftGenerator - ](T_TFlex_Model_Model3D_Geometry_LoftGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
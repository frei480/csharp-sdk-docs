

Руководство по T-FLEX CAD Open API

# LoftGeneratorSetFirstBody - метод  
  
---  
  
Функция тело с которого берутся касательные для начального профиля

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetFirstBody(
	BaseBody b,
	double sc
)
```
```vb
Public Sub SetFirstBody ( 
	b As BaseBody,
	sc As Double
)
```
```cpp
public:
void SetFirstBody(
	BaseBody^ b, 
	double sc
)
```


#### Параметры

b [BaseBody](T_TFlex_Model_Model3D_Geometry_BaseBody.md)
    Твёрдое тело с которого берутся касательные
sc [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Коэффициент масштабирования касательного вектора

#### Ссылки

[LoftGenerator - ](T_TFlex_Model_Model3D_Geometry_LoftGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)


Руководство по T-FLEX CAD Open API

# ShellGeneratorAddFace - метод  
    
Функция задаёт параметры отступа индивидуально для грани

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddFace(
	BaseTopol face,
	double dist
)
```
```vb
Public Sub AddFace ( 
	face As BaseTopol,
	dist As Double
)
```
```cpp
public:
void AddFace(
	BaseTopol^ face, 
	double dist
)
```


#### Параметры

face [BaseTopol](T_TFlex_Model_Model3D_Geometry_BaseTopol.md)
    Грань, для которой устанавливается отступ
dist [Double](https://learn.microsoft.com/dotnet/api/system.double)
    величина отступа в метрах

#### Ссылки

[ShellGenerator - ](T_TFlex_Model_Model3D_Geometry_ShellGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)


Руководство по T-FLEX CAD Open API

# Path3DCreate - метод  
  
---  
**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Path3D Create(
	Document document,
	List<BaseCurve> curves,
	List<BaseInterval> intervals
)
```
```vb
Public Shared Function Create ( 
	document As Document,
	curves As List(Of BaseCurve),
	intervals As List(Of BaseInterval)
) As Path3D
```
```cpp
public:
static Path3D^ Create(
	Document^ document, 
	List<BaseCurve^>^ curves, 
	List<BaseInterval^>^ intervals
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    
curves [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[BaseCurve](T_TFlex_Model_Model3D_Geometry_BaseCurve.md)
    
intervals [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[BaseInterval](T_TFlex_Model_Model3D_Geometry_BaseInterval.md)
    

#### Возвращаемое значение

[Path3D](T_TFlex_Model_Model3D_Path3D.md)

#### Ссылки

[Path3D - ](T_TFlex_Model_Model3D_Path3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
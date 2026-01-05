

Руководство по T-FLEX CAD Open API

# EdgeBlendinggetTopol - метод  
  
---  
  
Получить топологию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ModelTopol getTopol(
	int topolIndex
)
```
```vb
Public Function getTopol ( 
	topolIndex As Integer
) As ModelTopol
```
```cpp
public:
ModelTopol^ getTopol(
	int topolIndex
)
```


#### Параметры

topolIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер топологии

#### Возвращаемое значение

[ModelTopol](T_TFlex_Model_Model3D_Geometry_ModelTopol.md)Топология

Топология может быть ребром, циклом или гранью

#### Ссылки

[EdgeBlending - ](T_TFlex_Model_Model3D_EdgeBlending.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
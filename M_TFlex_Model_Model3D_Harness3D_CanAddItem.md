

Руководство по T-FLEX CAD Open API

# Harness3DCanAddItem - метод  
  
---  
  
Проверяет возможность вставить элемент в жгут, критерий: нет входит в текущий жгут и поджгуты, не принадлежит другим жгутам

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool CanAddItem(
	Construction3D pElement
)
```
```vb
Public Function CanAddItem ( 
	pElement As Construction3D
) As Boolean
```
```cpp
public:
bool CanAddItem(
	Construction3D^ pElement
)
```


#### Параметры

pElement [Construction3D](T_TFlex_Model_Model3D_Construction3D.md)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

#### Ссылки

[Harness3D - ](T_TFlex_Model_Model3D_Harness3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
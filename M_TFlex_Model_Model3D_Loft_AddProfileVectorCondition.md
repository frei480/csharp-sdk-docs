

Руководство по T-FLEX CAD Open API

# LoftAddProfileVectorCondition - метод  
    
Добавить векторное условие на профиле

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddProfileVectorCondition(
	int profileIndex,
	LoftVectorCondition condition
)
```
```vb
Public Sub AddProfileVectorCondition ( 
	profileIndex As Integer,
	condition As LoftVectorCondition
)
```
```cpp
public:
void AddProfileVectorCondition(
	int profileIndex, 
	LoftVectorCondition^ condition
)
```


#### Параметры

profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Индекс профиля
condition [LoftVectorCondition](T_TFlex_Model_Model3D_Loft_VectorCondition.md)
    Векторное граничное условие

Векторные граничные условия не могут быть заданы, если для данного профиля задан другой тип граничного условия

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
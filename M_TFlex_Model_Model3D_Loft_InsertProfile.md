

Руководство по T-FLEX CAD Open API

# LoftInsertProfile - метод  
  
---  
  
Вставить профиль в список профилей

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void InsertProfile(
	int profileIndex,
	ModelContour contour
)
```
```vb
Public Sub InsertProfile ( 
	profileIndex As Integer,
	contour As ModelContour
)
```
```cpp
public:
void InsertProfile(
	int profileIndex, 
	ModelContour^ contour
)
```


#### Параметры

profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер добавляемого профиля (начинается с 0)
contour [ModelContour](T_TFlex_Model_Model3D_Geometry_ModelContour.md)
    

После добавления профиля его нужно наполнить контурами с помощью функции AddProfileContour. Операция Лофтинга должна иметь как минимум один невырожденный профиль заданный с помощью контуров

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)

[AddProfile(ModelContour)](M_TFlex_Model_Model3D_Loft_AddProfile.md)

[RemoveProfile(Int32)](M_TFlex_Model_Model3D_Loft_RemoveProfile.md)
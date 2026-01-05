

Руководство по T-FLEX CAD Open API

# ViewSectionViewPointsArrayDelete - метод  
  
---  
  
Удалить точку по номеру

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Delete(
	int Index
)
```
```vb
Public Sub Delete ( 
	Index As Integer
)
```
```cpp
public:
void Delete(
	int Index
)
```


#### Параметры

Index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат неопределён

#### Ссылки

[ViewSectionViewPointsArray - ](T_TFlex_Model_Model3D_ViewSection_ViewPointsArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
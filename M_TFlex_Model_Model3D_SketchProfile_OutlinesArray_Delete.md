

Руководство по T-FLEX CAD Open API

# SketchProfileOutlinesArrayDelete - метод  
  
---  
  
Удалить линию изображения по номеру

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Delete(
	int index
)
```
```vb
Public Sub Delete ( 
	index As Integer
)
```
```cpp
public:
void Delete(
	int index
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер линии изображения

Линии изображения нумеруются от нуля. Если индекс отрицательный или превышает количество линий изображения, то результат не определён

#### Ссылки

[SketchProfileOutlinesArray - ](T_TFlex_Model_Model3D_SketchProfile_OutlinesArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
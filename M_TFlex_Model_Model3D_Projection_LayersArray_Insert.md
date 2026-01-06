

Руководство по T-FLEX CAD Open API

# ProjectionLayersArrayInsert - метод  
    
Вставить слой перед номером

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void Insert(
	int index,
	string layer
)
```




#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер слоя
layer [String](https://learn.microsoft.com/dotnet/api/system.string)
    Вставляемый слой

Слои нумеруются от нуля. Если индекс отрицательный или превышает количество слоёв, то результат не определён

#### Ссылки

[ProjectionLayersArray - ](T_TFlex_Model_Model3D_Projection_LayersArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
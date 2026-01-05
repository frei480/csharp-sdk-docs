

Руководство по T-FLEX CAD Open API

# ProjectionOutlineArrayItem - свойство  
  
---  
  
Получить элемент по номеру

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
protected ProjectionOutline this[
	int index
] { get; }
```
```vb
Protected ReadOnly Property Item ( 
	index As Integer
) As ProjectionOutline
	Get
```
```cpp
protected:
property ProjectionOutline^ Item[int index] {
	ProjectionOutline^ get (int index);
}
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Значение свойства

[ProjectionOutline](T_TFlex_Model_Model3D_ProjectionOutline.md)

Элементы нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат неопределён

#### Ссылки

[ProjectionOutlineArray - ](T_TFlex_Model_Model3D_ProjectionOutlineArray.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
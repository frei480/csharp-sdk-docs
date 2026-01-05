

Руководство по T-FLEX CAD Open API

# TableFunctionDelete - метод  
  
---  
  
Удалить точку по номеру

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
    Номер точки

Точки нумеруются от нуля. Если индекс отрицательный или превышает количество точек, то результат не определён

#### Ссылки

[TableFunction - ](T_TFlex_Model_Model3D_TableFunction.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
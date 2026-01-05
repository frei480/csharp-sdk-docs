

Руководство по T-FLEX CAD Open API

# SpiralSetStartSmooth - метод  
  
---  
  
Установить параметры сглаживания начальных витков

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetStartSmooth(
	Parameter smooth,
	Parameter degree
)
```
```vb
Public Sub SetStartSmooth ( 
	smooth As Parameter,
	degree As Parameter
)
```
```cpp
public:
void SetStartSmooth(
	Parameter^ smooth, 
	Parameter^ degree
)
```


#### Параметры

smooth [Parameter](T_TFlex_Model_Parameter.md)
    Число сглаживаемых витков
degree [Parameter](T_TFlex_Model_Parameter.md)
    Число сглаживаемых витков

Все значения должны быть нулевыми, или ненулевыми

#### Ссылки

[Spiral - ](T_TFlex_Model_Model3D_Spiral.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
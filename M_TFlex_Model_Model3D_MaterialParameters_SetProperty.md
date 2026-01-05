

Руководство по T-FLEX CAD Open API

# MaterialParametersSetProperty - метод  
  
---  
  
Установка физических параметров материала

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetProperty(
	MaterialParametersPhysicalProperty prop,
	Parameter parameter
)
```
```vb
Public Sub SetProperty ( 
	prop As MaterialParametersPhysicalProperty,
	parameter As Parameter
)
```
```cpp
public:
void SetProperty(
	MaterialParametersPhysicalProperty prop, 
	Parameter^ parameter
)
```


#### Параметры

prop [MaterialParametersPhysicalProperty](T_TFlex_Model_Model3D_MaterialParameters_PhysicalProperty.md)
    Свойство материала
parameter [Parameter](T_TFlex_Model_Parameter.md)
    Физический параметер

Единицы измерения параметра в завимости от типа свойства: Плотность (Density) TFlex.Model.Units.StandardUnits.Density.KilogramPerCubicMillimeter Модуль упругости (E_x, E_y, E_z) TFlex.Model.Units.StandardUnits.BreakingStrength.NewtonPerSquareMillimeter Коэффициент Пуассона (Nu_yz, Nu_xz,Nu_xy) безразмерный Модуль сдвига (G_xy, G_yz, G_xz) TFlex.Model.Units.StandardUnits.BreakingStrength.NewtonPerSquareMillimeter Коэффициент линейного расширения (Alpha_) TFlex.Model.Units.StandardUnits.ThermalExpansionCoefficient._1PerDegree Теплопроводность (K_x, K_y, K_z) TFlex.Model.Units.StandardUnits.ThermalConductivity.WattPerMillimeterDegree Предел прочности на разрыв (Sigma_ T) TFlex.Model.Units.StandardUnits.BreakingStrength.NewtonPerSquareMillimeter Предел прочности на сжатие (Sigma_ C) TFlex.Model.Units.StandardUnits.BreakingStrength.NewtonPerSquareMillimeter Предел текучести (Sigma_ Yield) TFlex.Model.Units.StandardUnits.BreakingStrength.NewtonPerSquareMillimeter Удельная теплоемкость (specific_heat) TFlex.Model.Units.StandardUnits.SpecificHeatCapacity.JoulePerKilogramKelvin Предел прочности на сдвиг (Tau_ ) TFlex.Model.Units.StandardUnits.BreakingStrength.NewtonPerSquareMillimeter 

#### Ссылки

[MaterialParameters - ](T_TFlex_Model_Model3D_MaterialParameters.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
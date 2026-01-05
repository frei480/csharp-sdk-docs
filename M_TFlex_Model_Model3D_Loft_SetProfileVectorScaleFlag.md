

Руководство по T-FLEX CAD Open API

# LoftSetProfileVectorScaleFlag - метод  
  
---  
  
Устанавливает параметр использования коэффициента касательного вектора как масштабного

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetProfileVectorScaleFlag(
	int profileIndex,
	bool scaleFlag
)
```
```vb
Public Sub SetProfileVectorScaleFlag ( 
	profileIndex As Integer,
	scaleFlag As Boolean
)
```
```cpp
public:
void SetProfileVectorScaleFlag(
	int profileIndex, 
	bool scaleFlag
)
```


#### Параметры

profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер профиля реверс которого возвращается
scaleFlag [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    true - интерпретирвать значение как масштабный коэффициент false - интерпретировать значение как длину

По умолчанию параметр отключен

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)


Руководство по T-FLEX CAD Open API

# LoftSetGuideVectorScaleFlag - метод  
    
Устанавливает параметр использования коэффициента касательного вектора как масштабного

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetGuideVectorScaleFlag(
	int guideIndex,
	bool scale
)
```
```vb
Public Sub SetGuideVectorScaleFlag ( 
	guideIndex As Integer,
	scale As Boolean
)
```
```cpp
public:
void SetGuideVectorScaleFlag(
	int guideIndex, 
	bool scale
)
```


#### Параметры

guideIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер направляющей реверс которого возвращается
scale [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    true - интерпретировать значение как масштабный коэффициент, false - интерпретировать значение как длину

По умолчанию параметр отключен

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
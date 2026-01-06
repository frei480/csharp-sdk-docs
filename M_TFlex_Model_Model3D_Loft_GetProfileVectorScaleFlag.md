

Руководство по T-FLEX CAD Open API

# LoftGetProfileVectorScaleFlag - метод  
    
Возвращает параметр интерпретации коэффициента касательного вектора

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool GetProfileVectorScaleFlag(
	int profileIndex
)
```
```vb
Public Function GetProfileVectorScaleFlag ( 
	profileIndex As Integer
) As Boolean
```
```cpp
public:
bool GetProfileVectorScaleFlag(
	int profileIndex
)
```


#### Параметры

profileIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер профиля для которого задаётся параметр

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Если параметр не установлен (по умолчанию), то коэффициент интерпретируется как длина вектора, если параметр установлен то коэффициент интерпретируется как масштабный коэффициент

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
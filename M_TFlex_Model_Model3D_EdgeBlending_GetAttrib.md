

Руководство по T-FLEX CAD Open API

# EdgeBlendingGetAttrib - метод  
    
Получить атрибуты топологии

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public EdgeBlendingAttribute GetAttrib(
	int topolIndex
)
```
```vb
Public Function GetAttrib ( 
	topolIndex As Integer
) As EdgeBlendingAttribute
```
```cpp
public:
EdgeBlendingAttribute^ GetAttrib(
	int topolIndex
)
```


#### Параметры

topolIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер топологии

#### Возвращаемое значение

[EdgeBlendingAttribute](T_TFlex_Model_Model3D_EdgeBlending_Attribute.md)

Если атрибут равен 0, тогда топология использует общие атрибуты

#### Ссылки

[EdgeBlending - ](T_TFlex_Model_Model3D_EdgeBlending.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
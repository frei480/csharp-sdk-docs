

Руководство по T-FLEX CAD Open API

# EdgeBlendingSetAttrib - метод  
    
Установить атрибуты топологии

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetAttrib(
	int topolIndex,
	EdgeBlendingAttribute attrib
)
```




#### Параметры

topolIndex [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер топологии
attrib [EdgeBlendingAttribute](T_TFlex_Model_Model3D_EdgeBlending_Attribute.md)
    Атрибуты

Если attrib равно 0, тогда топология использует общие атрибуты. Параметр Position для первой и последней позиции, не используется и изменяется

#### Ссылки

[EdgeBlending - ](T_TFlex_Model_Model3D_EdgeBlending.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
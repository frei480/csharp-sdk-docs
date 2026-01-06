

Руководство по T-FLEX CAD Open API

# LoftCanSetAutomaticCouplingPoint - метод  
    
Узнать можно ли установить автоматические точки соответствия

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool CanSetAutomaticCouplingPoint()
```
```vb
Public Function CanSetAutomaticCouplingPoint As Boolean
```
```cpp
public:
bool CanSetAutomaticCouplingPoint()
```


#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)

Автоматические точки соответствия могут быть установлены при выполнении следующих условий: 1\. Все контуры плоские. 2\. Все контуры замкнуты. 3\. Все или все кроме одного контуры профилей являются G1-непрерывными.

#### Ссылки

[Loft - ](T_TFlex_Model_Model3D_Loft.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
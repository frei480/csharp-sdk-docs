

Руководство по T-FLEX CAD Open API

# DecorationCircleArc(String, FloatVector, FloatVector, FloatVector) - конструктор  
    
Конструктор

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public DecorationCircleArc(
	string name,
	FloatVector center,
	FloatVector start,
	FloatVector end
)
```
```vb
Public Sub New ( 
	name As String,
	center As FloatVector,
	start As FloatVector,
	end As FloatVector
)
```
```cpp
public:
DecorationCircleArc(
	String^ name, 
	FloatVector center, 
	FloatVector start, 
	FloatVector end
)
```


#### Параметры

name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя должно быть уникальным
center [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Центр окружности
start [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Начало дуги
end [FloatVector](T_TFlex_Model_Model3D_FloatVector.md)
    Конец дуги

#### Значение поля

Создает дугу окружности по центру, началу и концу дуги 

#### Ссылки

[DecorationCircleArc - ](T_TFlex_Model_Model3D_Visual_DecorationCircleArc.md)

[DecorationCircleArc - перегрузка](Overload_TFlex_Model_Model3D_Visual_DecorationCircleArc__ctor.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)
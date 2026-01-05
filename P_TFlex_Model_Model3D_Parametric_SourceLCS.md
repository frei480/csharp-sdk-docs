

Руководство по T-FLEX CAD Open API

# ParametricSourceLCS - свойство  
  
---  
  
Исходная система координат

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public LCS SourceLCS { get; set; }
```
```vb
Public Property SourceLCS As LCS
	Get
	Set
```
```cpp
public:
property LCS^ SourceLCS {
	LCS^ get ();
	void set (LCS^ value);
}
```


#### Значение свойства

[LCS](T_TFlex_Model_Model3D_LCS.md)

К каждой копии применяется преобразование из исходной системы координат в текущую, которая может быть расчитана по пути или задана явными функциональными зависимостями от номера копии. Исходная система координат может быть задана явно. Если исходная ЛСК не задана, то в качестве исходной ЛСК используется ЛСК первой копии

#### Ссылки

[Parametric - ](T_TFlex_Model_Model3D_Parametric.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
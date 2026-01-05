

Руководство по T-FLEX CAD Open API

# Fragment3DFixByFragmentLCS - метод  
  
---  
  
Привязать фрагмент по системе координат, существующей в документе фрагмента к системе координат в сборке

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void FixByFragmentLCS(
	string sourceLCSName,
	LCS targetLCS
)
```
```vb
Public Sub FixByFragmentLCS ( 
	sourceLCSName As String,
	targetLCS As LCS
)
```
```cpp
public:
void FixByFragmentLCS(
	String^ sourceLCSName, 
	LCS^ targetLCS
)
```


#### Параметры

sourceLCSName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя системы координат, созданной в документе фрагмента
targetLCS [LCS](T_TFlex_Model_Model3D_LCS.md)
    Система координат, созданная в документе сборки(может быть **null**)

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
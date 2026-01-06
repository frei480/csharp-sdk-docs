

Руководство по T-FLEX CAD Open API

# Picture3DFixByPictureLCS - метод  
    
Привязать 3D изображение по системе координат созданной в документе фрагмента в систему координат сборки 

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void FixByPictureLCS(
	string sourceLCSName,
	LCS targetLCS
)
```
```vb
Public Sub FixByPictureLCS ( 
	sourceLCSName As String,
	targetLCS As LCS
)
```
```cpp
public:
void FixByPictureLCS(
	String^ sourceLCSName, 
	LCS^ targetLCS
)
```


#### Параметры

sourceLCSName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя системы координат, созданной в документе фрагмента
targetLCS [LCS](T_TFlex_Model_Model3D_LCS.md)
    Система координат, созданная в документе сборки

#### Ссылки

[Picture3D - ](T_TFlex_Model_Model3D_Picture3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
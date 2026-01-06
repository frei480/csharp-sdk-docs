

Руководство по T-FLEX CAD Open API

# MaterialGetFromLibrary - метод  
    
Получить объект "Материал" с указанным именем из библиотеки

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static Material GetFromLibrary(
	Document document,
	string name
)
```
```vb
Public Shared Function GetFromLibrary ( 
	document As Document,
	name As String
) As Material
```
```cpp
public:
static Material^ GetFromLibrary(
	Document^ document, 
	String^ name
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ, в котором создаётся новый объект
name [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя материала

#### Возвращаемое значение

[Material](T_TFlex_Model_Model3D_Material.md)Материал

#### Ссылки

[Material - ](T_TFlex_Model_Model3D_Material.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
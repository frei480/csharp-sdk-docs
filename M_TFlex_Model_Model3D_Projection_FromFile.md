

Руководство по T-FLEX CAD Open API

# ProjectionFromFile - метод  
    
Создание проекции из файла

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool FromFile(
	string path,
	string version
)
```
```vb
Public Function FromFile ( 
	path As String,
	version As String
) As Boolean
```
```cpp
public:
bool FromFile(
	String^ path, 
	String^ version
)
```


#### Параметры

path [String](https://learn.microsoft.com/dotnet/api/system.string)
    
version [String](https://learn.microsoft.com/dotnet/api/system.string)
    

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Возвращает true - если файл по указанному пути может быть использован для проецирования

#### Ссылки

[Projection - ](T_TFlex_Model_Model3D_Projection.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
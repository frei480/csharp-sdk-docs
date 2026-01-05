

Руководство по T-FLEX CAD Open API

# Fragment3DIncludeInSpecificBom - свойство  
  
---  
  
Включение в спецификацию

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public IncludeInBom this[
	string bomName
] { get; set; }
```
```vb
Public Property IncludeInSpecificBom ( 
	bomName As String
) As IncludeInBom
	Get
	Set
```
```cpp
public:
property IncludeInBom IncludeInSpecificBom[String^ bomName] {
	IncludeInBom get (String^ bomName);
	void set (String^ bomName, IncludeInBom value);
}
```


#### Параметры

bomName [String](https://learn.microsoft.com/dotnet/api/system.string)
    

#### Значение свойства

[IncludeInBom](T_TFlex_Model_IncludeInBom.md)

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
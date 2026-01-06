

Руководство по T-FLEX CAD Open API

# MaterialParametersTextureFileName - свойство  
    
Имя файла текстуры

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public string TextureFileName { get; set; }
```
```vb
Public Property TextureFileName As String
	Get
	Set
```
```cpp
public:
property String^ TextureFileName {
	String^ get ();
	void set (String^ value);
}
```


#### Значение свойства

[String](https://learn.microsoft.com/dotnet/api/system.string)

Пустое имя означает отсутствие текстуры. Поддерживаются форматы файлов: GIF, JPEG, BMP, PNG. Для возможности экспорта в формат VRML рекомендуется использовать JPEG или PNG

#### Ссылки

[MaterialParameters - ](T_TFlex_Model_Model3D_MaterialParameters.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
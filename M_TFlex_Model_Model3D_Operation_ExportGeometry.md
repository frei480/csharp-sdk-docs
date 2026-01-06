

Руководство по T-FLEX CAD Open API

# OperationExportGeometry - метод  
    
Сохранение тел в файл в формате Parasolid

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public bool ExportGeometry(
	string file,
	bool redundant,
	bool materials,
	bool assembly,
	bool binary
)
```




#### Параметры

file [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя выходного файла
redundant [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Удалять избыточную геометрию
materials [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Выгружать с материалами
assembly [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Сохранять структуру сборки
binary [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать бинарный формат

#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Результат экспорта

#### Ссылки

[Operation - ](T_TFlex_Model_Model3D_Operation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
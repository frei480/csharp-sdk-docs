

Руководство по T-FLEX CAD Open API

# Fragment3DGetFragmentDocument(Boolean, Boolean) - метод  
    
Получить документ фрамента с подстановкой значений переменных фрагмента

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Document GetFragmentDocument(
	bool substitute,
	bool update
)
```
```vb
Public Function GetFragmentDocument ( 
	substitute As Boolean,
	update As Boolean
) As Document
```
```cpp
public:
Document^ GetFragmentDocument(
	bool substitute, 
	bool update
)
```


#### Параметры

substitute [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Признак необходимости подстановки значений переменных
update [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Обновить документ фрагмента

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Документ фрагмента

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[GetFragmentDocument - перегрузка](Overload_TFlex_Model_Model3D_Fragment3D_GetFragmentDocument.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
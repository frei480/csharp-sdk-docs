

Руководство по T-FLEX CAD Open API

# Fragment3D(String, Document, Boolean, Boolean) - конструктор  
    
Конструктор для создания 3D фрагмента

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Fragment3D(
	string fileName,
	Document document,
	bool copy,
	bool autoSave
)
```
```vb
Public Sub New ( 
	fileName As String,
	document As Document,
	copy As Boolean,
	autoSave As Boolean
)
```
```cpp
public:
Fragment3D(
	String^ fileName, 
	Document^ document, 
	bool copy, 
	bool autoSave
)
```


#### Параметры

fileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя файла документа фрагмента
document [Document](T_TFlex_Model_Document.md)
    Документ, в котором создаётся новый объект
copy [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать файл как шаблон для создания нового документа фрагмента в оперативной памяти
autoSave [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Создавать фрагмент в режиме автосохранения

#### Ссылки

[Fragment3D - ](T_TFlex_Model_Model3D_Fragment3D.md)

[Fragment3D - перегрузка](Overload_TFlex_Model_Model3D_Fragment3D__ctor.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
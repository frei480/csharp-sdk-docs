

Руководство по T-FLEX CAD Open API

# Fragment(Document, String, Boolean, Boolean) - конструктор  
  
---  
  
Конструктор с именем файла фрагмента

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public Fragment(
	Document document,
	string filePath,
	bool copy,
	bool autoSave
)
```
```vb
Public Sub New ( 
	document As Document,
	filePath As String,
	copy As Boolean,
	autoSave As Boolean
)
```
```cpp
public:
Fragment(
	Document^ document, 
	String^ filePath, 
	bool copy, 
	bool autoSave
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ объекта
filePath [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя файла фрагмента
copy [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Использовать файл как шаблон для создания нового документа фрагмента в оперативной памяти
autoSave [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Создавать фрагмент в режиме автосохранения

#### Ссылки

[Fragment - ](T_TFlex_Model_Model2D_Fragment.md)

[Fragment - перегрузка](Overload_TFlex_Model_Model2D_Fragment__ctor.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
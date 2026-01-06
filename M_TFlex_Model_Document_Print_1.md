

Руководство по T-FLEX CAD Open API

# DocumentPrint(IntPtr, Boolean, Boolean) - метод  
    
Печать документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Print(
	IntPtr window,
	bool selectAllPages,
	bool fitAndCenter
)
```
```vb
Public Sub Print ( 
	window As IntPtr,
	selectAllPages As Boolean,
	fitAndCenter As Boolean
)
```
```cpp
public:
void Print(
	IntPtr window, 
	bool selectAllPages, 
	bool fitAndCenter
)
```


#### Параметры

window [IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)
    Родительское окно
selectAllPages [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Выбрать все страницы, иначе - только активную
fitAndCenter [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Центрировать и вписать в страницу
    
    
    public static void DocPrint(IntPtr window)
    {
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
    
       bool selectAllPages = true; //true-выбрать все страницы, false - только активную
       bool fitAndCenter = true;//Центрировать и вписать в страницу
       //метод вызывает диалоговое окно.
       document.Print(window, selectAllPages, fitAndCenter);
       //document.PrintNoDialog(); //печать без диалгового окна
    }

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[Print - перегрузка](Overload_TFlex_Model_Document_Print.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
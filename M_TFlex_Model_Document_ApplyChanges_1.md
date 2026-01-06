

Руководство по T-FLEX CAD Open API

# DocumentApplyChanges(Boolean) - метод  
    
Применить изменения без закрытия блока изменения документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public ChangesResult ApplyChanges(
	bool regenerate3D
)
```
```vb
Public Function ApplyChanges ( 
	regenerate3D As Boolean
) As ChangesResult
```
```cpp
public:
ChangesResult ApplyChanges(
	bool regenerate3D
)
```


#### Параметры

regenerate3D [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Переcчитать 3D документ

#### Возвращаемое значение

[ChangesResult](T_TFlex_Model_ChangesResult.md)Результат применения изменений

Функция применяет изменения, сделаные после вызова функции [BeginChanges(String)](M_TFlex_Model_Document_BeginChanges.md). В зависимости от параметра regenerate3D пересчитывает или нет 3D документ

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[ApplyChanges - перегрузка](Overload_TFlex_Model_Document_ApplyChanges.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
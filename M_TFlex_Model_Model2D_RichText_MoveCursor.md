

Руководство по T-FLEX CAD Open API

# RichTextMoveCursor - метод  
    
Перемещение курсора на несколько символов вперёд или назад

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void MoveCursor(
	int charactersCount
)
```




#### Параметры

charactersCount [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Количество символов

Если значение параметра charactersCount больше 0, то курсор будет перемещён вперёд на charactersCount символов. Если значение параметра charactersCount меньше 0, то курсор будет перемещён на абсолютное значение charactersCount символов

#### Ссылки

[RichText - ](T_TFlex_Model_Model2D_RichText.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)


Руководство по T-FLEX CAD Open API

# RibbonButton - класс  
    
Кнопка на ленте T-FLEX CAD

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlexRibbonButton

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public sealed class RibbonButton : IDisposable
```
```vb
Public NotInheritable Class RibbonButton
	Implements IDisposable
```
```cpp
public ref class RibbonButton sealed : IDisposable
```


Тип RibbonButton предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [Caption](P_TFlex_RibbonButton_Caption.md) | Отображаемый на кнопке текст |
|  | [ChildButton](P_TFlex_RibbonButton_ChildButton.md) | i-ая кнопка, вложенная в эту |
|  | [ChildButtonCount](P_TFlex_RibbonButton_ChildButtonCount.md) | Количество кнопок, вложенных в эту |
|  | [ChildButtons](P_TFlex_RibbonButton_ChildButtons.md) | Кнопки, вложенные в эту |
|  | [Description](P_TFlex_RibbonButton_Description.md) | Описание команды, выполняемой при нажатии на эту кнопку |
|  | [ID](P_TFlex_RibbonButton_ID.md) | Идентификатор этой кнопки |
|  | [Style](P_TFlex_RibbonButton_Style.md) |  |
|  | [ToolTip](P_TFlex_RibbonButton_ToolTip.md) | Текст подсказки, отображаемой при наведении курсора на эту кнопку |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddChildButton(Int32)](M_TFlex_RibbonButton_AddChildButton.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [AddChildButton(Int32, String)](M_TFlex_RibbonButton_AddChildButton_1.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [AddChildButton(Int32, Plugin)](M_TFlex_RibbonButton_AddChildButton_5.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [AddChildButton(Int32, RibbonButtonStyle)](M_TFlex_RibbonButton_AddChildButton_7.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [AddChildButton(Int32, String, Plugin)](M_TFlex_RibbonButton_AddChildButton_2.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [AddChildButton(Int32, String, RibbonButtonStyle)](M_TFlex_RibbonButton_AddChildButton_4.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [AddChildButton(Int32, Plugin, RibbonButtonStyle)](M_TFlex_RibbonButton_AddChildButton_6.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [AddChildButton(Int32, String, Plugin, RibbonButtonStyle)](M_TFlex_RibbonButton_AddChildButton_3.md) | Добавляет кнопку в список кнопок, вложенных в эту |
|  | [Dispose](M_TFlex_RibbonButton_Dispose.md) | Освобождает все ресурсы, используемые объектом RibbonButton |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Remove](M_TFlex_RibbonButton_Remove.md) | Удаляет эту кнопку из содержащего её контейнера (группы ленты или другой кнопки) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex - пространство имён](N_TFlex.md)


Руководство по T-FLEX CAD Open API

# ValueChangedEventArgs - класс  
    
Событие изменения значения NumericInputControl

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [SystemEventArgs](https://learn.microsoft.com/dotnet/api/system.eventargs) [TFlex.DialogsBaseEventArgs](T_TFlex_Dialogs_BaseEventArgs.md) TFlex.DialogsValueChangedEventArgs

**Пространство имён:** [TFlex.Dialogs](N_TFlex_Dialogs.md)**Сборка:** TFlexCommandAPI (в TFlexCommandAPI.dll) Версия: 17.1.20.0

```csharp
public class ValueChangedEventArgs : BaseEventArgs
```




Тип ValueChangedEventArgs предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [ClampedValue](P_TFlex_Dialogs_ValueChangedEventArgs_ClampedValue.md) | Возвращает новое числовое значение (в границах) |
|  | [Handled](P_TFlex_Dialogs_BaseEventArgs_Handled.md) | Помечает событие как обработанное(Унаследован от [BaseEventArgs](T_TFlex_Dialogs_BaseEventArgs.md)) |
|  | [IsStateChanged](P_TFlex_Dialogs_ValueChangedEventArgs_IsStateChanged.md) | Возвращает true, если состояние (State) изменилось |
|  | [IsUnitChanged](P_TFlex_Dialogs_ValueChangedEventArgs_IsUnitChanged.md) | Возвращает true, если единица измерения изменилась |
|  | [IsUnitConverted](P_TFlex_Dialogs_ValueChangedEventArgs_IsUnitConverted.md) | Возвращает true, если единица измерения изменилась в результате конвертации |
|  | [IsValid](P_TFlex_Dialogs_ValueChangedEventArgs_IsValid.md) | Возвращает новое значение IsValid |
|  | [IsValueChanged](P_TFlex_Dialogs_ValueChangedEventArgs_IsValueChanged.md) | Возвращает true, если значение изменилось |
|  | [IsVariableChanged](P_TFlex_Dialogs_ValueChangedEventArgs_IsVariableChanged.md) | Возвращает true, если переменная изменилась |
|  | [State](P_TFlex_Dialogs_ValueChangedEventArgs_State.md) | Возвращает новое состояние (State) |
|  | [Unit](P_TFlex_Dialogs_ValueChangedEventArgs_Unit.md) | Возвращает новую единицу измерения |
|  | [Value](P_TFlex_Dialogs_ValueChangedEventArgs_Value.md) | Возвращает новое числовое значение |
|  | [Variable](P_TFlex_Dialogs_ValueChangedEventArgs_Variable.md) | Возвращает новую переменную |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Dialogs - пространство имён](N_TFlex_Dialogs.md)
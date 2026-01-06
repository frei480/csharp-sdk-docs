

Руководство по T-FLEX CAD Open API

# FragmentVariableValue - класс  
    
Класс предназначенный для задания значения переменной фрагмента

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.ModelFragmentVariableValue

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public class FragmentVariableValue : IDisposable
```




Тип FragmentVariableValue предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [AttachedNode](P_TFlex_Model_FragmentVariableValue_AttachedNode.md) | Узел сборки, связанный с внешней переменной |
|  | [AttachedVariable](P_TFlex_Model_FragmentVariableValue_AttachedVariable.md) | Выражение для внешней переменной |
|  | [IsReal](P_TFlex_Model_FragmentVariableValue_IsReal.md) | Проверка, является ли переменная вещественной |
|  | [IsSet](P_TFlex_Model_FragmentVariableValue_IsSet.md) | Задано ли значение переменной. Если значение не задано, то оно определяется значением переменной внутри документа фрагмента. |
|  | [IsText](P_TFlex_Model_FragmentVariableValue_IsText.md) | Проверка, является ли переменная текстовой |
|  | [IsValueFromConnector](P_TFlex_Model_FragmentVariableValue_IsValueFromConnector.md) | Установлено ли значение переменной в соответствии со значением этой переменной в коннекторе |
|  | [Name](P_TFlex_Model_FragmentVariableValue_Name.md) | Имя переменной |
|  | [OriginalRealValue](P_TFlex_Model_FragmentVariableValue_OriginalRealValue.md) | Вещественное значение переменной из документа фрагмента |
|  | [OriginalTextValue](P_TFlex_Model_FragmentVariableValue_OriginalTextValue.md) | Текстовое значение переменной из документа фрагмента |
|  | [RealValue](P_TFlex_Model_FragmentVariableValue_RealValue.md) | Вещественное значение переменной |
|  | [TextValue](P_TFlex_Model_FragmentVariableValue_TextValue.md) | Текстовое значение переменной |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Dispose](M_TFlex_Model_FragmentVariableValue_Dispose.md) | Освобождает все ресурсы, используемые объектом FragmentVariableValue |
|  | [Dispose(Boolean)](M_TFlex_Model_FragmentVariableValue_Dispose_1.md) | Освобождает неуправляемые ресурсы, используемые объектом FragmentVariableValue, а при необходимости освобождает также управляемые ресурсы |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [Finalize](M_TFlex_Model_FragmentVariableValue_Finalize.md) | (Переопределяет [ObjectFinalize](https://learn.microsoft.com/dotnet/api/system.object.finalize)) |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetValueList](M_TFlex_Model_FragmentVariableValue_GetValueList.md) | Получить список значений, которые может принимать переменная, если он задан |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [SetDefaultValue](M_TFlex_Model_FragmentVariableValue_SetDefaultValue.md) | Установка значения переменной по умолчанию, на основе значения этой переменной внутри документа фрагмента |
|  | [SetValueFromConnector](M_TFlex_Model_FragmentVariableValue_SetValueFromConnector.md) | **Устарело.** Установка значения переменной в соотвествии со значением этой переменной в коннекторе, использованном для привязки фрагмента |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
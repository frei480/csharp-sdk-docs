

Руководство по T-FLEX CAD Open API

# ComparisonOperator - класс  
    
Оператор сравнения

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) TFlex.Model.Data.FiltersComparisonOperator

**Пространство имён:** [TFlex.Model.Data.Filters](N_TFlex_Model_Data_Filters.md)**Сборка:** TFlexAPIData (в TFlexAPIData.dll) Версия: 17.1.20.0 (17.1.20.0)

```csharp
public abstract class ComparisonOperator
```




Тип ComparisonOperator предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [RequireValueList](P_TFlex_Model_Data_Filters_ComparisonOperator_RequireValueList.md) | Возвращает значение, указывающее, должен ли быть операнд списком значений |
|  | [SupportsSecondOperand](P_TFlex_Model_Data_Filters_ComparisonOperator_SupportsSecondOperand.md) | Возвращает значение, указывающее, поддерживается ли оператором сравнения второй операнд |
|  | [Type](P_TFlex_Model_Data_Filters_ComparisonOperator_Type.md) | Возвращает тип оператора |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Compare](M_TFlex_Model_Data_Filters_ComparisonOperator_Compare.md) | Возвращает значение, указывающее, выполняется ли условие оператора сравнения для указанных операндов |
|  | [Equals](M_TFlex_Model_Data_Filters_ComparisonOperator_Equals.md) | Возвращает значение, указывающее, равен ли заданный объект текущему(Переопределяет [ObjectEquals(Object)](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\))) |
|  | [Finalize](https://learn.microsoft.com/dotnet/api/system.object.finalize) | Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetAllOperators](M_TFlex_Model_Data_Filters_ComparisonOperator_GetAllOperators.md) | Возвращает список всех операторов сравнения |
|  | [GetHashCode](M_TFlex_Model_Data_Filters_ComparisonOperator_GetHashCode.md) | Возвращает хэш-код оператора сравнения(Переопределяет [ObjectGetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode)) |
|  | [GetOperator](M_TFlex_Model_Data_Filters_ComparisonOperator_GetOperator.md) | Возвращает оператор сравнения по его типу |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [MemberwiseClone](https://learn.microsoft.com/dotnet/api/system.object.memberwiseclone) | Creates a shallow copy of the current [Object](https://learn.microsoft.com/dotnet/api/system.object).(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [ToString](M_TFlex_Model_Data_Filters_ComparisonOperator_ToString.md) | (Переопределяет [ObjectToString](https://learn.microsoft.com/dotnet/api/system.object.tostring)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Equality(ComparisonOperator, ComparisonOperator)](M_TFlex_Model_Data_Filters_ComparisonOperator_op_Equality.md) | Определяет, равны ли указанные операции |
|  | [Inequality(ComparisonOperator, ComparisonOperator)](M_TFlex_Model_Data_Filters_ComparisonOperator_op_Inequality.md) | Определяет, различаются ли указанные операции |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [ContainsSubstring](F_TFlex_Model_Data_Filters_ComparisonOperator_ContainsSubstring.md) | Возвращает оператор "Содержит" |
|  | [EndsWithSubstring](F_TFlex_Model_Data_Filters_ComparisonOperator_EndsWithSubstring.md) | Возвращает оператор "Заканчивается на" |
|  | [Equal](F_TFlex_Model_Data_Filters_ComparisonOperator_Equal.md) | Возвращает оператор "=" |
|  | [GreaterThan](F_TFlex_Model_Data_Filters_ComparisonOperator_GreaterThan.md) | Возвращает оператор ">" |
|  | [GreaterThanOrEqual](F_TFlex_Model_Data_Filters_ComparisonOperator_GreaterThanOrEqual.md) | Возвращает оператор ">=" |
|  | [IsEmptyString](F_TFlex_Model_Data_Filters_ComparisonOperator_IsEmptyString.md) | Возвращает оператор "Не содержит текст" |
|  | [IsNotEmptyString](F_TFlex_Model_Data_Filters_ComparisonOperator_IsNotEmptyString.md) | Возвращает оператор "Содержит текст" |
|  | [IsNotNull](F_TFlex_Model_Data_Filters_ComparisonOperator_IsNotNull.md) | Возвращает оператор "Содержит какие-либо данные" |
|  | [IsNotOneOf](F_TFlex_Model_Data_Filters_ComparisonOperator_IsNotOneOf.md) | Возвращает оператор "Не входит в список" |
|  | [IsNull](F_TFlex_Model_Data_Filters_ComparisonOperator_IsNull.md) | Возвращает оператор "Не содержит данных" |
|  | [IsOneOf](F_TFlex_Model_Data_Filters_ComparisonOperator_IsOneOf.md) | Возвращает оператор "Входит в список" |
|  | [LessThan](F_TFlex_Model_Data_Filters_ComparisonOperator_LessThan.md) | Возвращает оператор "<" |
|  | [LessThanOrEqual](F_TFlex_Model_Data_Filters_ComparisonOperator_LessThanOrEqual.md) | Возвращает оператор "<=" |
|  | [MatchMask](F_TFlex_Model_Data_Filters_ComparisonOperator_MatchMask.md) | Возвращает оператор "Соответствует маске" |
|  | [NotContainSubstring](F_TFlex_Model_Data_Filters_ComparisonOperator_NotContainSubstring.md) | Возвращает оператор "Не содержит" |
|  | [NotEqual](F_TFlex_Model_Data_Filters_ComparisonOperator_NotEqual.md) | Возвращает оператор "!=" |
|  | [NotMatchMask](F_TFlex_Model_Data_Filters_ComparisonOperator_NotMatchMask.md) | Возвращает оператор "Не соответствует маске" |
|  | [StartsWithSubstring](F_TFlex_Model_Data_Filters_ComparisonOperator_StartsWithSubstring.md) | Возвращает оператор "Начинается с" |
  
#### Ссылки

[TFlex.Model.Data.Filters - пространство имён](N_TFlex_Model_Data_Filters.md)
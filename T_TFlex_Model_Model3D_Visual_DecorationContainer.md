

Руководство по T-FLEX CAD Open API

# DecorationContainer - класс  
    
Контейнер декораций

[SystemObject](https://learn.microsoft.com/dotnet/api/system.object) [TFlex.Model.Model3D.VisualDecoration](T_TFlex_Model_Model3D_Visual_Decoration.md) TFlex.Model.Model3D.VisualDecorationContainer

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public sealed class DecorationContainer : Decoration, 
	IEnumerable
```
```vb
Public NotInheritable Class DecorationContainer
	Inherits Decoration
	Implements IEnumerable
```
```cpp
public ref class DecorationContainer sealed : public Decoration, 
	IEnumerable
```


Тип DecorationContainer предоставляет следующие члены.

|  | Имя | Описание |
| --- | --- | --- |
|  | [DecorationContainer](M_TFlex_Model_Model3D_Visual_DecorationContainer__ctor.md) | Инициализирует новый экземпляр класса DecorationContainer |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [Name](P_TFlex_Model_Model3D_Visual_Decoration_Name.md) | Имя декорации(Унаследован от [Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)) |
  
|  | Имя | Описание |
| --- | --- | --- |
|  | [AddDecoration](M_TFlex_Model_Model3D_Visual_DecorationContainer_AddDecoration.md) | Добавление декорации |
|  | [Dispose](M_TFlex_Model_Model3D_Visual_Decoration_Dispose.md) | (Унаследован от [Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)) |
|  | [Equals](https://learn.microsoft.com/dotnet/api/system.object.equals#system-object-equals\(system-object\)) | Determines whether the specified object is equal to the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetDecoration](M_TFlex_Model_Model3D_Visual_DecorationContainer_GetDecoration.md) | Поиск декорации |
|  | [GetEnumerator](M_TFlex_Model_Model3D_Visual_DecorationContainer_GetEnumerator.md) | Реализация интерфейса IEnumerable |
|  | [GetHashCode](https://learn.microsoft.com/dotnet/api/system.object.gethashcode) | Serves as the default hash function. (Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [GetType](https://learn.microsoft.com/dotnet/api/system.object.gettype) | Gets the [Type](https://learn.microsoft.com/dotnet/api/system.type) of the current instance.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
|  | [IsEmpty](M_TFlex_Model_Model3D_Visual_DecorationContainer_IsEmpty.md) | Проверка пустоты |
|  | [RemoveAllDecorations](M_TFlex_Model_Model3D_Visual_DecorationContainer_RemoveAllDecorations.md) | Удаление всех декораций |
|  | [RemoveDecoration](M_TFlex_Model_Model3D_Visual_DecorationContainer_RemoveDecoration.md) | Удаление декорации |
|  | [ToString](https://learn.microsoft.com/dotnet/api/system.object.tostring) | Returns a string that represents the current object.(Унаследован от [Object](https://learn.microsoft.com/dotnet/api/system.object)) |
  
Позволяет группировать несколько декораций Не допускается модифицировать контейнер декораций, который был получен от системы, а не создан явным образом.

#### Ссылки

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)

[DecorationManager](T_TFlex_Model_Model3D_Visual_DecorationManager.md)

[DecorationShape](T_TFlex_Model_Model3D_Visual_DecorationShape.md)
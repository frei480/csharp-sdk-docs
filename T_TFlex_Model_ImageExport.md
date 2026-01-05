

Руководство по T-FLEX CAD Open API

# ImageExport - перечисление  
  
---  
  
Опции экспорта изображений

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[FlagsAttribute]
public enum ImageExport
```
```vb
<FlagsAttribute>
Public Enumeration ImageExport
```
```cpp
[FlagsAttribute]
public enum class ImageExport
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| None | 0 | Не экспортировать вспомогательные объекты |
| ScreenLayers | 1 | Экспортировать экранные слои |
| Constructions | 2 | Экспортировать элементы построения |
| Constraints | 4 | Экспортировать ограничения |
| InternalTest | 8 |  |
| Default | 241 | Экспортировать все элементы, кроме элементов построения и ограничений |
  
#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
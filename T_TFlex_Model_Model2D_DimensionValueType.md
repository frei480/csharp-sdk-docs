

Руководство по T-FLEX CAD Open API

# DimensionValueType - перечисление  
    
Способы формирования строки номинала размера

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum DimensionValueType
```




| Имя члена | Значение | Описание |
| --- | --- | --- |
| NoNominal | 0 | Нет номинала |
| AutoCount | 1 | Расчет |
| Manual | 2 | Вручную |
| FromExtraData | 3 | Обозначение берётся из дополнительных данных с родительских объектов |
| From3dParent | 4 | С родительского 3D размера |
| Control | 7 | Управляющий |
| FromSourceObjects | 100 | Расчет по исходным объектам (для размеров на ассоциативных копиях) |
  
#### Ссылки

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
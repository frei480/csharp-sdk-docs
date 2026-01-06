

Руководство по T-FLEX CAD Open API

# ProjectionProjectionsElements - перечисление  
    
Выбор проецируемых элементов или элементов, к которым применяется сечение

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[FlagsAttribute]
public enum ProjectionsElements
```




| Имя члена | Значение | Описание |
| --- | --- | --- |
| AllOperations | 1 | Все операции |
| OnlySelectedElements | 2 | Все выбранные элементы ( по умолчанию ) |
| AllWithTheExceptionOfSelectedOperations | 4 | Все операции за исключением выбранных операций |
| File | 16 | Тела из файла |
| OperationAllTypes | 23 | Все типы операций |
| AllWelds | 32 | Все сварные швы |
| OnlySelectedWelds | 64 | Все выбранные сварные швы ( по умолчанию ) |
| AllWithTheExceptionOfSelectedWelds | 128 | Все сварные швы за исключением выбранных сварных швов |
| AllProfiles | 256 | Все профили |
| OnlySelectedProfiles | 512 | Все выбранные профили ( по умолчанию ) |
| AllWithTheExceptionOfSelectedProfiles | 1,024 | Все профили за исключением выбранных профилей |
| ProfileAllTypes | 1,792 | Все типы профилей |
| AllPaths | 2,048 | Все пути |
| OnlySelectedPaths | 4,096 | Все выбранные пути ( по умолчанию ) |
| AllWithTheExceptionOfSelectedPaths | 8,192 | Все пути за исключением выбранных путей |
| PathAllTypes | 14,336 | Все типы путей |
| AllLcs | 16,384 | Все системы координат |
| OnlySelectedLcs | 32,768 | Все выбранные системы координат ( по умолчанию ) |
| AllWithTheExceptionOfSelectedLcs | 65,536 | Все системы координат за исключением выбранных систем координат |
| LcsAllTypes | 114,688 | Все типы систем координат |
| TopolsAllTypes | 131,072 | Геометрические элементы |
| OperationWelds | 262,144 | Также как в операциях |
| WeldAllTypes | 262,368 | Все типы сварных швов |
| AllAxis | 1,048,576 | Все оси |
| OnlySelectedAxis | 2,097,152 | Все выбранные оси ( по умолчанию ) |
| AllWithTheExceptionOfSelectedAxis | 4,194,304 | Все оси за исключением выбранных осей |
| AxisAllTypes | 7,340,032 | Все типы осей |
| AllSomeElements | 9,455,905 | Все элементы одного из типов |
| OnlySelectedSomeElements | 18,911,810 | Выбранные элементы |
| AllWithTheExceptionOfSelectedSomeElements | 37,823,620 | Все элементы за исключением выбранных |
| ProjectionsElementsNewTypes | 66,584,544 | Все новые типы |
| ProjectionsElementsAllTypes | 66,584,567 | Все типы |
  
#### Ссылки

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
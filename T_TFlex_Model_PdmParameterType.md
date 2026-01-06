

Руководство по T-FLEX CAD Open API

# PdmParameterType - перечисление  
    
Тип параметра PDM системы

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum PdmParameterType
```




| Имя члена | Значение | Описание |
| --- | --- | --- |
| None | 0 | Не определён |
| Nomenclature | 1 | Номенклатура |
| Document | 2 | Документ |
| File | 3 | Файл |
| ConfigurationSettings | 4 | Параметры конфигурации |
      
    
    public static void VariableToDOCs()
    {
       Document doc = TFlex.Application.ActiveDocument;//Получение активного документа
       doc.BeginChanges("Передача параметров в DOCs");//Открытие блока изменений документа
    
       //создание переменной
       TFlex.Model.Variable var = new TFlex.Model.Variable(doc, "$xxx", "111");
       //Строка описания параметра PDM системы - в виде Guid
       var.PdmParameterDescription = "[262a61a6-ca61-4404-9131-ddb992230c31]";
       //Направление передачи параметров при интеграции с PDM - в обе стороны
       var.PdmConnectionDirection = PdmConnectionDirection.Both;
       //Тип параметра PDM системы - параметр файла
       var.PdmParameterType = PdmParameterType.File;
    
       doc.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[TFlex.Model - пространство имён](N_TFlex_Model.md)
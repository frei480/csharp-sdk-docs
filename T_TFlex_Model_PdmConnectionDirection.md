

Руководство по T-FLEX CAD Open API

# PdmConnectionDirection - перечисление  
  
---  
  
Направление передачи параметров при интеграции с PDM

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public enum PdmConnectionDirection
```
```vb
Public Enumeration PdmConnectionDirection
```
```cpp
public enum class PdmConnectionDirection
```


| Имя члена | Значение | Описание |
| --- | --- | --- |
| Both | 0 | двустороняя передача |
| FromPdm | 1 | из PDM |
| FromCad | 2 | из CAD |
      
    
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


Руководство по T-FLEX CAD Open API

# ApplicationNewAnnotation - метод  
    
Создать новую аннотацию для указанного файла документа

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static Document NewAnnotation(
	string documentFileName,
	Annotation annotation
)
```




#### Параметры

documentFileName [String](https://learn.microsoft.com/dotnet/api/system.string)
    Путь к файлу аннотируемого документа
annotation [Annotation](T_TFlex_Annotation.md)
    Параметры создаваемой аннотации с указанием пути к файлу

#### Возвращаемое значение

[Document](T_TFlex_Model_Document.md)Созданный документ аннотации или null в случае ошибки

#### Ссылки

[Application - ](T_TFlex_Application.md)

[TFlex - пространство имён](N_TFlex.md)
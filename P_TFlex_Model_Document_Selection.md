

Руководство по T-FLEX CAD Open API

# DocumentSelection - свойство  
  
---  
  
Селектор документа

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public SelectionContainer Selection { get; }
```
```vb
Public ReadOnly Property Selection As SelectionContainer
	Get
```
```cpp
public:
property SelectionContainer^ Selection {
	SelectionContainer^ get ();
}
```


#### Значение свойства

[SelectionContainer](T_TFlex_Model_SelectionContainer.md)

Объект класса [SelectionContainer](T_TFlex_Model_SelectionContainer.md). может быть 0 в случае если документ не имеет селектора. Не иметь селектора может, например, документ, используемый в качестве фрагмента.

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
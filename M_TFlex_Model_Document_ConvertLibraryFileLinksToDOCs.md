

Руководство по T-FLEX CAD Open API

# DocumentConvertLibraryFileLinksToDOCs - метод  
  
---  
  
**Примечание: Данный API устарел.**

Переназначить ссылки на файлы в библиотеке T-Flex CAD на ссылки в библиотеке DOCs

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This method is obsolete. Only for T-FLEX DOCs 11. Please use Variable Properties: PdmParameterDescription, PdmConnectionDirection, PdmParameterType.")]
public void ConvertLibraryFileLinksToDOCs(
	IntPtr hDOCsHandle
)
```
```vb
<ObsoleteAttribute("This method is obsolete. Only for T-FLEX DOCs 11. Please use Variable Properties: PdmParameterDescription, PdmConnectionDirection, PdmParameterType.")>
Public Sub ConvertLibraryFileLinksToDOCs ( 
	hDOCsHandle As IntPtr
)
```
```cpp
public:
[ObsoleteAttribute(L"This method is obsolete. Only for T-FLEX DOCs 11. Please use Variable Properties: PdmParameterDescription, PdmConnectionDirection, PdmParameterType.")]
void ConvertLibraryFileLinksToDOCs(
	IntPtr hDOCsHandle
)
```


#### Параметры

hDOCsHandle [IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)
    Идентификатор документа DOCs

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
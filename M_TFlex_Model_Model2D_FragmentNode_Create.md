

Руководство по T-FLEX CAD Open API

# FragmentNodeCreate - метод  
  
---  
  
Создание узла в указанном документе, соответствующего заданному узлу элемента, находящегося на вложенном фрагменте

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static FragmentNode Create(
	Document document,
	Fragment[] arrPath,
	Object2D sourceElement,
	int id
)
```
```vb
Public Shared Function Create ( 
	document As Document,
	arrPath As Fragment(),
	sourceElement As Object2D,
	id As Integer
) As FragmentNode
```
```cpp
public:
static FragmentNode^ Create(
	Document^ document, 
	array<Fragment^>^ arrPath, 
	Object2D^ sourceElement, 
	int id
)
```


#### Параметры

document [Document](T_TFlex_Model_Document.md)
    Документ
arrPath [Fragment](T_TFlex_Model_Model2D_Fragment.md)
    Массив вложенных фрагментов
sourceElement [Object2D](T_TFlex_Model_Model2D_Object2D.md)
    Заданный элемент
id [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Идентификатор узла элемента

#### Возвращаемое значение

[FragmentNode](T_TFlex_Model_Model2D_FragmentNode.md)Созданный объект

0-й фрагмент в массиве - должен быть вложен в указанный документ. Заданный объект должен находиться на последнем фрагменте массива. В данный момент возможно создание узла на конце (id=1) или в начале (id=0) линии построения.

#### Ссылки

[FragmentNode - ](T_TFlex_Model_Model2D_FragmentNode.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
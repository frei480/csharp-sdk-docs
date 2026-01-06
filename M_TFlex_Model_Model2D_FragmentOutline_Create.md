

Руководство по T-FLEX CAD Open API

# FragmentOutlineCreate - метод  
    
Создание элемента в указанном документе, соответствующего заданному элементу, находящегося на вложенном фрагменте

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static FragmentOutline Create(
	Document doc,
	Fragment[] arrPath,
	Outline sourceElement
)
```




#### Параметры

doc [Document](T_TFlex_Model_Document.md)
    Документ
arrPath [Fragment](T_TFlex_Model_Model2D_Fragment.md)
    Массив вложенных фрагментов
sourceElement [Outline](T_TFlex_Model_Model2D_Outline.md)
    Заданный элемент

#### Возвращаемое значение

[FragmentOutline](T_TFlex_Model_Model2D_FragmentOutline.md)Созданный объект

0-й фрагмент в массиве - должен быть вложен в указанный документ. Заданный объект должен находиться на последнем фрагменте массива.

#### Ссылки

[FragmentOutline - ](T_TFlex_Model_Model2D_FragmentOutline.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
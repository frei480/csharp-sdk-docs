

Руководство по T-FLEX CAD Open API

# ViewSectionPoints - свойство  
    
Множество точек. Ломанная, построенная на последовательности проекций этих точек на плоскость сечения образуют контур сечения

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public ViewSectionViewPointsArray Points { get; }
```
```vb
Public ReadOnly Property Points As ViewSectionViewPointsArray
	Get
```
```cpp
public:
property ViewSectionViewPointsArray^ Points {
	ViewSectionViewPointsArray^ get ();
}
```


#### Значение свойства

[ViewSectionViewPointsArray](T_TFlex_Model_Model3D_ViewSection_ViewPointsArray.md)

В настоящей версии в качестве точки можно выбирать только 3D узлы и вершины. В остальных случаях сечение строится не будет

#### Ссылки

[ViewSection - ](T_TFlex_Model_Model3D_ViewSection.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
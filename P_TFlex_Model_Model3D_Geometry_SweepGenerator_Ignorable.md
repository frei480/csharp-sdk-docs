

Руководство по T-FLEX CAD Open API

# SweepGeneratorIgnorable - свойство  
  
---  
  
Получить множество игнорируемых вершин траектории.

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SweepGeneratorIgnorableVertices Ignorable { get; }
```
```vb
Public ReadOnly Property Ignorable As SweepGeneratorIgnorableVertices
	Get
```
```cpp
public:
property SweepGeneratorIgnorableVertices^ Ignorable {
	SweepGeneratorIgnorableVertices^ get ();
}
```


#### Значение свойства

[SweepGeneratorIgnorableVertices](T_TFlex_Model_Model3D_Geometry_SweepGenerator_IgnorableVertices.md)

В некоторых случаях при формировании граней можно в местах сочленения сегментов тела, соответсвующих вершинам траектории, избежать построения рёбер, сшивая грани в одну. Если не задан тип разбиения результирущего тела на грани Grid, то такая обработка выполняется автоматически. Если задан тип Grid, то можно задать набор вершин траектории, для которых будет выполняться такая обработка. В данный список нельзя добавлять первую и последнюю вершины размкутой траектории или вершины, где смежные рёбра траектории не G1 - непрерывны

#### Ссылки

[SweepGenerator - ](T_TFlex_Model_Model3D_Geometry_SweepGenerator.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
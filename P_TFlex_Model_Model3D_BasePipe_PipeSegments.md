

Руководство по T-FLEX CAD Open API

# BasePipePipeSegments - свойство  
  
---  
  
**Примечание: Данный API устарел.**

Возвращает информацию об участках трубопровода

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("Do not call this method. Use property this.Path.Path3DSegments")]
public BasePipePipeSegment[] PipeSegments { get; }
```
```vb
<ObsoleteAttribute("Do not call this method. Use property this.Path.Path3DSegments")>
Public ReadOnly Property PipeSegments As BasePipePipeSegment()
	Get
```
```cpp
public:
[ObsoleteAttribute(L"Do not call this method. Use property this.Path.Path3DSegments")]
property array<BasePipePipeSegment^>^ PipeSegments {
	array<BasePipePipeSegment^>^ get ();
}
```


#### Значение свойства

[BasePipePipeSegment](T_TFlex_Model_Model3D_BasePipe_PipeSegment.md)

#### Ссылки

[BasePipe - ](T_TFlex_Model_Model3D_BasePipe.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
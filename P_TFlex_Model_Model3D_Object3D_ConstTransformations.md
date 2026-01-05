

Руководство по T-FLEX CAD Open API

# Object3DConstTransformations - свойство  
  
---  
  
**Примечание: Данный API устарел.**

Преобразование 3D объекта для чтения (устаревшая версия трансформации - допускается чтение трансформации в старых документах.)

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("The property is obsolete. Use Transformations instead.")]
public TransformationContainer ConstTransformations { get; }
```
```vb
<ObsoleteAttribute("The property is obsolete. Use Transformations instead.")>
Public ReadOnly Property ConstTransformations As TransformationContainer
	Get
```
```cpp
public:
[ObsoleteAttribute(L"The property is obsolete. Use Transformations instead.")]
property TransformationContainer^ ConstTransformations {
	TransformationContainer^ get ();
}
```


#### Значение свойства

[TransformationContainer](T_TFlex_Model_Model3D_TransformationContainer.md)

#### Ссылки

[Object3D - ](T_TFlex_Model_Model3D_Object3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
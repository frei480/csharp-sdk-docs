

Руководство по T-FLEX CAD Open API

# PipePath3DAddSegment_backType \- метод  
  
---  
  
**Примечание: Данный API устарел.**

Добавить участок в конец

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("This method is obsolete and will be removed. Please use 'AddBackSegment' method.")]
public Type AddSegment_back<Type>(
	SegmentPipePathType type
)
where Type : PipePath3DBaseSegment

```
```vb
<ObsoleteAttribute("This method is obsolete and will be removed. Please use 'AddBackSegment' method.")>
Public Function AddSegment_back(Of Type As PipePath3DBaseSegment) ( 
	type As SegmentPipePathType
) As Type
```
```cpp
public:
[ObsoleteAttribute(L"This method is obsolete and will be removed. Please use 'AddBackSegment' method.")]
generic<typename Type>
where Type : PipePath3DBaseSegment
Type AddSegment_back(
	SegmentPipePathType type
)
```


#### Параметры

type [SegmentPipePathType](T_TFlex_Model_Model3D_SegmentPipePathType.md)
    

#### Параметры типа

Type
    

#### Возвращаемое значение

Type

#### Ссылки

[PipePath3D - ](T_TFlex_Model_Model3D_PipePath3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
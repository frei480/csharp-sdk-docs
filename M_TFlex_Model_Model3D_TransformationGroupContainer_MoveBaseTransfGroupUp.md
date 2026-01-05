

Руководство по T-FLEX CAD Open API

# TransformationGroupContainerMoveBaseTransfGroupUp - метод  
  
---  
  
Переместить базовую группу трансформаций на 1 позицию вверх. В случае успеха transfGroup становится устаревшей (IsValid == false).

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public TransformationGroup MoveBaseTransfGroupUp(
	TransformationGroup transfGroup
)
```
```vb
Public Function MoveBaseTransfGroupUp ( 
	transfGroup As TransformationGroup
) As TransformationGroup
```
```cpp
public:
TransformationGroup^ MoveBaseTransfGroupUp(
	TransformationGroup^ transfGroup
)
```


#### Параметры

transfGroup [TransformationGroup](T_TFlex_Model_Model3D_TransformationGroup.md)
    перемещаемая группа

#### Возвращаемое значение

[TransformationGroup](T_TFlex_Model_Model3D_TransformationGroup.md)возвращает обновленную группу преобразований.

после вызова этого метода полученные ранее объекты групп трансформаций TransformationGroup могут ссылаться на другие группы.

#### Ссылки

[TransformationGroupContainer - ](T_TFlex_Model_Model3D_TransformationGroupContainer.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
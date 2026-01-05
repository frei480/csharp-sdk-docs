

Руководство по T-FLEX CAD Open API

# BoundedExtrusionGeneratorBound(Boolean, BaseFace, Boolean, UInt32, BoundedExtrusionGeneratorBoundSideType) - конструктор  
  
---  
  
Конструктор для задания границы гранью

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Bound(
	bool forward,
	BaseFace face,
	bool nearest,
	uint division,
	BoundedExtrusionGeneratorBoundSideType side
)
```
```vb
Public Sub New ( 
	forward As Boolean,
	face As BaseFace,
	nearest As Boolean,
	division As UInteger,
	side As BoundedExtrusionGeneratorBoundSideType
)
```
```cpp
public:
Bound(
	bool forward, 
	BaseFace^ face, 
	bool nearest, 
	unsigned int division, 
	BoundedExtrusionGeneratorBoundSideType side
)
```


#### Параметры

forward [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Граница задаётся в направлении вектора выталкивания ( true ) или в обратном направлении ( false )
face [BaseFace](T_TFlex_Model_Model3D_Geometry_BaseFace.md)
    Граничная грань
nearest [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    Если true, то разбиения нумеруются начиная с первого и увеличиваясь в направлении движения от профиля. Если false, то первое разбиение наиболее удалено от профиля и номер разбиения увеличивается в направлении движения к профилю
division [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Номер разбиения. Разбиения нумеруются от 1
side [BoundedExtrusionGeneratorBoundSideType](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound_SideType.md)
    Какая сторона ограничивающей грани, пересекающая профиль, считается первым разбиением. Для первого и последнего разбиений грани с твёрдого тела допустимыми значениями являются только In и Out

#### Ссылки

[BoundedExtrusionGeneratorBound - ](T_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound.md)

[BoundedExtrusionGeneratorBound - перегрузка](Overload_TFlex_Model_Model3D_Geometry_BoundedExtrusionGenerator_Bound__ctor.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
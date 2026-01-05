

Руководство по T-FLEX CAD Open API

# SheetFromTrimmedSurfaceLump - конструктор  
  
---  
  
Конструктор для связанной области

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Lump(
	SheetFromTrimmedSurfaceLumpLoop[] loops,
	uint id
)
```
```vb
Public Sub New ( 
	loops As SheetFromTrimmedSurfaceLumpLoop(),
	id As UInteger
)
```
```cpp
public:
Lump(
	array<SheetFromTrimmedSurfaceLumpLoop^>^ loops, 
	unsigned int id
)
```


#### Параметры

loops [SheetFromTrimmedSurfaceLumpLoop](T_TFlex_Model_Model3D_Geometry_SheetFromTrimmedSurface_Lump_Loop.md)
    Множество составных кривых, образующих границы связанной области
id [UInt32](https://learn.microsoft.com/dotnet/api/system.uint32)
    Идентификатор грани, уникальный в границах каждого 3D объекта внешнего приложения

Использование уникальных и воспроизводимых при каждом пересчёте объекта идентификаторов граней, позволяет обеспечить ассоциативность модели на уровне отдельных элементов топологии. Только одна составная кривая включает все остальные. Все кривые лежащие внутри не могут включать друг друга. Не допускается пересечение или касание между кривыми. Внешний цикл ориентирован против часовой стрелки. Внутренние циклы ориентированы по часовой стрелке

#### Ссылки

[SheetFromTrimmedSurfaceLump - ](T_TFlex_Model_Model3D_Geometry_SheetFromTrimmedSurface_Lump.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
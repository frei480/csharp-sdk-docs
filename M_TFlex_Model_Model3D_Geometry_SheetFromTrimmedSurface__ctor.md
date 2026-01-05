

Руководство по T-FLEX CAD Open API

# SheetFromTrimmedSurface - конструктор  
  
---  
  
Конструктор для задания листового тела на поверхности по набору параметрических составных кривых

**Пространство имён:** [TFlex.Model.Model3D.Geometry](N_TFlex_Model_Model3D_Geometry.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public SheetFromTrimmedSurface(
	ProxyObject3D object,
	BaseSurface surface,
	SheetFromTrimmedSurfaceLump[] lumps
)
```
```vb
Public Sub New ( 
	object As ProxyObject3D,
	surface As BaseSurface,
	lumps As SheetFromTrimmedSurfaceLump()
)
```
```cpp
public:
SheetFromTrimmedSurface(
	ProxyObject3D^ object, 
	BaseSurface^ surface, 
	array<SheetFromTrimmedSurfaceLump^>^ lumps
)
```


#### Параметры

object [ProxyObject3D](T_TFlex_Model_Model3D_ProxyObject3D.md)
    3D объект внешнего приложения, для которого генерируется результат
surface [BaseSurface](T_TFlex_Model_Model3D_Geometry_BaseSurface.md)
    Поверхность, на которой лежит листовое тело
lumps [SheetFromTrimmedSurfaceLump](T_TFlex_Model_Model3D_Geometry_SheetFromTrimmedSurface_Lump.md)
    Множество связанных областей

Все параметры обязательные. 3D объект внешнего приложения должен быть связан с внешним объектом

#### Ссылки

[SheetFromTrimmedSurface - ](T_TFlex_Model_Model3D_Geometry_SheetFromTrimmedSurface.md)

[TFlex.Model.Model3D.Geometry - пространство имён](N_TFlex_Model_Model3D_Geometry.md)
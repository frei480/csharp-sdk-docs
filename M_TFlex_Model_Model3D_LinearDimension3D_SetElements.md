

Руководство по T-FLEX CAD Open API

# LinearDimension3DSetElements - метод  
    
Установка привязок размера к 3D элементам

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void SetElements(
	Object3D Element1,
	Dimension3DElementType Element1Type,
	Object3D Element2,
	Dimension3DElementType Element2Type,
	DimensionUVCoords Coords
)
```




#### Параметры

Element1 [Object3D](T_TFlex_Model_Model3D_Object3D.md)
    1-й элемент размера (грань, ребро, узел)
Element1Type [Dimension3DElementType](T_TFlex_Model_Model3D_Dimension3DElementType.md)
    Тип 1-го элемента размера
Element2 [Object3D](T_TFlex_Model_Model3D_Object3D.md)
    2-й элемент размера (грань, ребро, узел)
Element2Type [Dimension3DElementType](T_TFlex_Model_Model3D_Dimension3DElementType.md)
    Тип 2-го элемента размера
Coords [DimensionUVCoords](T_TFlex_Model_Model3D_DimensionUVCoords.md)
    Координаты для определения привязки размера

#### Ссылки

[LinearDimension3D - ](T_TFlex_Model_Model3D_LinearDimension3D.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
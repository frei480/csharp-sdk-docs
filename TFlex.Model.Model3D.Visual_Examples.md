# Примеры использования классов в пространстве имён TFlex.Model.Model3D.Visual

## Описание пространства имён

Пространство имён `TFlex.Model.Model3D.Visual` содержит классы для визуализации 3D-моделей.

## Основные классы

### LCSWorkplane

**Пример создания рабочей плоскости:**
```csharp
LCSWorkplane workplane = new LCSWorkplane(document);
workplane.LCS = customLCS;

// Добавление трансформаций
TransformationGroup group = workplane.Transformations.AddBaseTransfGroup();
group.AddRotateTransf(TransformationCoordinate.X, 45.0);
```

### VisualStyle

**Пример настройки стиля отображения:**
```csharp
VisualStyle style = new VisualStyle();
style.Color = Color.Red;
style.LineWidth = 2.0;
style.ShowEdges = true;
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D.Visual_Examples.md
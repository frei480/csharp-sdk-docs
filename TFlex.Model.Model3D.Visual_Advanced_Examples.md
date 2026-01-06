# Продвинутые примеры использования классов в пространстве имён TFlex.Model.Model3D.Visual

## Расширенная визуализация

### Настройка стилей отображения

```csharp
public void ConfigureAdvancedVisualStyles()
{
    VisualStyle wireframeStyle = new VisualStyle();
    wireframeStyle.RenderMode = RenderMode.Wireframe;
    wireframeStyle.LineColor = Color.Blue;
    wireframeStyle.LineWidth = 1.5f;
    
    VisualStyle shadedStyle = new VisualStyle();
    shadedStyle.RenderMode = RenderMode.Shaded;
    shadedStyle.Material = new Material(Color.Gray, 0.8f);
    shadedStyle.ShowEdges = true;
}
```

### Работа с камерой

```csharp
public void SetupCameraView()
{
    Camera camera = new Camera();
    camera.Position = new Point3D(100, 100, 100);
    camera.Target = new Point3D(0, 0, 0);
    camera.UpVector = new Direction(0, 0, 1);
    camera.FieldOfView = 45.0;
    
    // Ортогональная проекция
    camera.ProjectionMode = ProjectionMode.Orthographic;
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D.Visual_Advanced_Examples.md
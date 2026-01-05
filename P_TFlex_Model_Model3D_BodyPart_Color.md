

Руководство по T-FLEX CAD Open API

# BodyPartColor - свойство  
  
---  
  
Цвет

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public Parameter Color { get; set; }
```
```vb
Public Property Color As Parameter
	Get
	Set
```
```cpp
public:
property Parameter^ Color {
	Parameter^ get ();
	void set (Parameter^ value);
}
```


#### Значение свойства

[Parameter](T_TFlex_Model_Parameter.md)
    
    
    public static void SetColor(Object ob)
    {            
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       ob.Color = 40;//установка цвета
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[BodyPart - ](T_TFlex_Model_Model3D_BodyPart.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
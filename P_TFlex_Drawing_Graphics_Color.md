

Руководство по T-FLEX CAD Open API

# GraphicsColor - свойство  
  
---  
  
Цвет, которым производится вывод

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public int Color { get; set; }
```
```vb
Public Property Color As Integer
	Get
	Set
```
```cpp
public:
property int Color {
	int get ();
	void set (int value);
}
```


#### Значение свойства

[Int32](https://learn.microsoft.com/dotnet/api/system.int32)

Предопределённые значения перечислены в перечислителе [Color](T_TFlex_Drawing_Color.md)
    
    
    public static void SetColor(Object ob)
    {            
       Document document = TFlex.Application.ActiveDocument;//Получение активного документа
       document.BeginChanges("");//Открытие блока изменений документа
    
       ob.Color = 40;//установка цвета
    
       document.EndChanges();//Закрытие блока изменений документа
    }

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
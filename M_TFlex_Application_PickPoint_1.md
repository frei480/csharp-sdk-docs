

Руководство по T-FLEX CAD Open API

# ApplicationPickPoint(PickPointParameters) - метод  
  
---  
  
Получить точку в одном из видов активного документа

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public static PickPointResult PickPoint(
	PickPointParameters parameters
)
```
```vb
Public Shared Function PickPoint ( 
	parameters As PickPointParameters
) As PickPointResult
```
```cpp
public:
static PickPointResult^ PickPoint(
	PickPointParameters^ parameters
)
```


#### Параметры

parameters [PickPointParameters](T_TFlex_PickPointParameters.md)
    Параметры ввода точки

#### Возвращаемое значение

[PickPointResult](T_TFlex_PickPointResult.md)Результат ввода точки
    
    
    using System;
    using System.Windows.Forms;
    
    using TFlex;
    using TFlex.Model;
    using TFlex.Model.Model2D;
    using TFlex.Model.Model3D;
    
    namespace NewMacroNamespace
    {
       public class NewMacroClass
       {
           public static void PickPoint()
           {
               PickPointParameters par = new PickPointParameters();
    
               //выбор только размеров
               SelectionFilter filter = new SelectionFilter();
               filter.Enable(ObjectType.Dimension);
               par.Filter = filter;
    
               par.Prompt = "Выбрать размер";
               par.MouseMove += new TFlex.PickPointMouseMove(PickPointMouseMove);//событие перемещения мыши
               PickPointResult res = TFlex.Application.PickPoint(par);//получить точку в одном из видов активного документа
    
               string mess = "Объект не выбран";
               if (res.SelectedObject != null)
               {
                   mess = string.Empty;
                   string val = string.Empty;
    
                   ObjectProperty[] arr = res.SelectedObject.GetProperties();//массив свойств выбранного объекта
                   for (int i = 0; i < arr.Length; i++)
                   {
                       switch (arr[i].Type)
                       {
                           case (ObjectPropertyType.IntProperty):
                               val = res.SelectedObject.GetIntProperty(arr[i].Name).Value.ToString();
                               break;
    
                           case (ObjectPropertyType.RealProperty):
                               val = res.SelectedObject.GetRealProperty(arr[i].Name).Value.ToString();
                               break;
    
                           case (ObjectPropertyType.TextProperty):
                               val = res.SelectedObject.GetTextProperty(arr[i].Name);
                               break;
                       }
    
                       mess += arr[i].Name + ": " + val + "\r\n";
                   }
               }
    
               MessageBox.Show(mess);
           }
    
           static public void PickPointMouseMove(Object sender, PickPointEventArgs e)
           {
           }
       }
    }

#### Ссылки

[Application - ](T_TFlex_Application.md)

[PickPoint - перегрузка](Overload_TFlex_Application_PickPoint.md)

[TFlex - пространство имён](N_TFlex.md)
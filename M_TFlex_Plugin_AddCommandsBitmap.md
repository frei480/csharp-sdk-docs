

Руководство по T-FLEX CAD Open API

# PluginAddCommandsBitmap - метод  
    
**Примечание: Данный API устарел.**

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
[ObsoleteAttribute("Not fully supported. Specify icons in RegisterCommand or RegisterObjectCommand instead.
To create toolbar use CreateToolbar.")]
protected void AddCommandsBitmap(
	Bitmap BmpSmall,
	Bitmap BmpLarge,
	int[] CmdIDs
)
```
```vb
<ObsoleteAttribute("Not fully supported. Specify icons in RegisterCommand or RegisterObjectCommand instead.
To create toolbar use CreateToolbar.")>
Protected Sub AddCommandsBitmap ( 
	BmpSmall As Bitmap,
	BmpLarge As Bitmap,
	CmdIDs As Integer()
)
```
```cpp
protected:
[ObsoleteAttribute(L"Not fully supported. Specify icons in RegisterCommand or RegisterObjectCommand instead.
To create toolbar use CreateToolbar.")]
void AddCommandsBitmap(
	Bitmap^ BmpSmall, 
	Bitmap^ BmpLarge, 
	array<int>^ CmdIDs
)
```


#### Параметры

BmpSmall [Bitmap](https://learn.microsoft.com/dotnet/api/system.drawing.bitmap)
    
BmpLarge [Bitmap](https://learn.microsoft.com/dotnet/api/system.drawing.bitmap)
    
CmdIDs [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Ссылки

[Plugin - ](T_TFlex_Plugin.md)

[TFlex - пространство имён](N_TFlex.md)
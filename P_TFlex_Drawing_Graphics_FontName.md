

Руководство по T-FLEX CAD Open API

# GraphicsFontName - свойство  
  
---  
  
Выбор шрифта для прорисовки текста

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public string FontName { set; }
```
```vb
Public WriteOnly Property FontName As String
	Set
```
```cpp
public:
property String^ FontName {
	void set (String^ value);
}
```


#### Значение свойства

[String](https://learn.microsoft.com/dotnet/api/system.string)

Тип шрифта зависит от расширения имени шрифта. Если присутствует расширение ".shx", то будет выбран шрифт формата SHX. Если выбирается шрифт типа TrueType (без расширения), то по умолчанию устанавливается стиль Normal из перечислителя [FontStyle](T_TFlex_Drawing_FontStyle.md). Метод [SetFontName(String, FontStyle)](M_TFlex_Drawing_Graphics_SetFontName.md) является альтернативой данному методу

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
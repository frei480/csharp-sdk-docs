

Руководство по T-FLEX CAD Open API

# GraphicsSetFontName - метод  
  
---  
  
Выбор шрифта для прорисовки текста

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetFontName(
	string fontname,
	FontStyle style
)
```
```vb
Public Sub SetFontName ( 
	fontname As String,
	style As FontStyle
)
```
```cpp
public:
void SetFontName(
	String^ fontname, 
	FontStyle style
)
```


#### Параметры

fontname [String](https://learn.microsoft.com/dotnet/api/system.string)
    Имя шрифта
style [FontStyle](T_TFlex_Drawing_FontStyle.md)
    Стиль шрифта. Учитывается только для шрифтов TrueType

Тип шрифта зависит от расширения имени шрифта. Если присутствует расширение".shx", то будет выбран шрифт формата SHX. Метод SetFontName(String, FontStyle) является альтернативой данному методу.

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
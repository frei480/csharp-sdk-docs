

Руководство по T-FLEX CAD Open API

# DocumentDraw - метод  
  
---  
  
Прорисовка указанной страниницы документа в указанный объект вывода графичесого изображения

**Пространство имён:** [TFlex.Model](N_TFlex_Model.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void Draw(
	Graphics graphics,
	Page pg
)
```
```vb
Public Sub Draw ( 
	graphics As Graphics,
	pg As Page
)
```
```cpp
public:
void Draw(
	Graphics^ graphics, 
	Page^ pg
)
```


#### Параметры

graphics [Graphics](T_TFlex_Drawing_Graphics.md)
    Объект вывода графичекого изображения
pg [Page](T_TFlex_Model_Page.md)
    Страница документа, которую необходимо вывести

#### Ссылки

[Document - ](T_TFlex_Model_Document.md)

[TFlex.Model - пространство имён](N_TFlex_Model.md)
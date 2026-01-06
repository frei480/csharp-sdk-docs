

Руководство по T-FLEX CAD Open API

# Главное окно системы  
    
Для доступа к главному окну T-FLEX CAD предназначен специальный класс [MainWindow](T_TFlex_MainWindow.md) и статический метод [Window](P_TFlex_Application_Window.md) для получения объекта этого класса. Данный класс предназначен для управления самим главным окном системы, а также его вспомогательными дочерними окнами.

Ниже приведен пример кода для подсчета количества видимых панелей инструментов.
```csharp
private int CountVisibleToolbars()
{
	//Инициализируем счетчик количества видимых панелей
	int count = 0;
	//Перебор всех панелей в окне приложения
	foreach(Toolbar toolbar in Application.Window.Toolbars)
	{
		//Если панель видимая,
		if(toolbar.Visible)
			//увеличиваем счетичик на единицу
			count++;
	}
	return count;
}
```
  
#### Ссылки

[Application](T_TFlex_Application.md)

Toolbar
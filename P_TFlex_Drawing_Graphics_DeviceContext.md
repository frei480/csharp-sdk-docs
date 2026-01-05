

Руководство по T-FLEX CAD Open API

# GraphicsDeviceContext - свойство  
  
---  
  
Установка дескриптора графического устройства (HDC)

**Пространство имён:** [TFlex.Drawing](N_TFlex_Drawing.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public IntPtr DeviceContext { get; set; }
```
```vb
Public Property DeviceContext As IntPtr
	Get
	Set
```
```cpp
public:
property IntPtr DeviceContext {
	IntPtr get ();
	void set (IntPtr value);
}
```


#### Значение свойства

[IntPtr](https://learn.microsoft.com/dotnet/api/system.intptr)

В некоторых случаях необходимо выводить изображение непосредственно на графическое устройство с использованием его дескриптора. Для этого используется данный метод. Для этого можно сконструировать объект данного класса со значением hWnd равным 0. Затем необходимо воспользоваться данным методом для установки дескриптора графического устройства. После завершения вывода обязательно обнуление дескриптора графического устройства. Для этого в качестве значения параметра hdc должно быть передано значение 0.

#### Ссылки

[Graphics - ](T_TFlex_Drawing_Graphics.md)

[TFlex.Drawing - пространство имён](N_TFlex_Drawing.md)
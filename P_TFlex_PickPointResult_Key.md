

Руководство по T-FLEX CAD Open API

# PickPointResultKey - свойство  
  
---  
  
Код клавиши, которая была нажата пользователем

**Пространство имён:** [TFlex](N_TFlex.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public KeyCode Key { get; set; }
```
```vb
Public Property Key As KeyCode
	Get
	Set
```
```cpp
public:
property KeyCode Key {
	KeyCode get ();
	void set (KeyCode value);
}
```


#### Значение свойства

[KeyCode](T_TFlex_KeyCode.md)

В случае нажатия левой кнопки мыши возвращается KeyKode.keyENTER. В случае нажатия правой кнопки мыши возвращается KeyKode.keyESCAPE. В последнем случае метод IsOK возвращает false.

#### Ссылки

[PickPointResult - ](T_TFlex_PickPointResult.md)

[TFlex - пространство имён](N_TFlex.md)
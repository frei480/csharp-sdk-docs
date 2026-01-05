

Руководство по T-FLEX CAD Open API

# DecorationManagerAddDecoration - метод  
  
---  
  
Регистрация декорации

**Пространство имён:** [TFlex.Model.Model3D.Visual](N_TFlex_Model_Model3D_Visual.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public void AddDecoration(
	Decoration decoration
)
```
```vb
Public Sub AddDecoration ( 
	decoration As Decoration
)
```
```cpp
public:
void AddDecoration(
	Decoration^ decoration
)
```


#### Параметры

decoration [Decoration](T_TFlex_Model_Model3D_Visual_Decoration.md)
    

Недопустимо регистрировать декорацию более одного раза. Декорации, связанные с манипулятором, не надо регистрировать. Для зарегистрированной декорации Dispose() вызывается автоматически. 

#### Ссылки

[DecorationManager - ](T_TFlex_Model_Model3D_Visual_DecorationManager.md)

[TFlex.Model.Model3D.Visual - пространство имён](N_TFlex_Model_Model3D_Visual.md)
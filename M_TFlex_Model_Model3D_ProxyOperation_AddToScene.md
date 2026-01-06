

Руководство по T-FLEX CAD Open API

# ProxyOperationAddToScene - метод  
    
Прогрузка операции в сцену

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
protected virtual bool AddToScene()
```
```vb
Protected Overridable Function AddToScene As Boolean
```
```cpp
protected:
virtual bool AddToScene()
```


#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Если операция реализует свою процедуру прогрузки, то нужно вернуть true

По умолчанию, прогружаются тела, полученные в MakeGeometry и добавленные в список тел при помощи AddSolid

#### Ссылки

[ProxyOperation - ](T_TFlex_Model_Model3D_ProxyOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
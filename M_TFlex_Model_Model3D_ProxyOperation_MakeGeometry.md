

Руководство по T-FLEX CAD Open API

# ProxyOperationMakeGeometry - метод  
  
---  
  
Пересчитать объект. Сформировать список тел в операции.

**Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
protected virtual bool MakeGeometry()
```
```vb
Protected Overridable Function MakeGeometry As Boolean
```
```cpp
protected:
virtual bool MakeGeometry()
```


#### Возвращаемое значение

[Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)Возвращается признак успешности выполнения пересчета

Тела добавлются с помощью функции AddSolid

#### Ссылки

[ProxyOperation - ](T_TFlex_Model_Model3D_ProxyOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
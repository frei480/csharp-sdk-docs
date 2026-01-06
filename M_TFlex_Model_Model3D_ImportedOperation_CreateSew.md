

Руководство по T-FLEX CAD Open API

# ImportedOperationCreateSew - метод  
  **Пространство имён:** [TFlex.Model.Model3D](N_TFlex_Model_Model3D.md)**Сборка:** TFlexAPI3D (в TFlexAPI3D.dll) Версия: 17.1.20.0

```csharp
public static ImportedOperation CreateSew(
	Document document,
	List<Operation> operations,
	double gap_width_bound,
	bool solid,
	ref List<int> exclude
)
```




#### Параметры

document [Document](T_TFlex_Model_Document.md)
    
operations [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[Operation](T_TFlex_Model_Model3D_Operation.md)
    
gap_width_bound [Double](https://learn.microsoft.com/dotnet/api/system.double)
    
solid [Boolean](https://learn.microsoft.com/dotnet/api/system.boolean)
    
exclude [List](https://learn.microsoft.com/dotnet/api/system.collections.generic.list-1)[Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    

#### Возвращаемое значение

[ImportedOperation](T_TFlex_Model_Model3D_ImportedOperation.md)

#### Ссылки

[ImportedOperation - ](T_TFlex_Model_Model3D_ImportedOperation.md)

[TFlex.Model.Model3D - пространство имён](N_TFlex_Model_Model3D.md)
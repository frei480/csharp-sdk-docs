

Руководство по T-FLEX CAD Open API

# FragmentSetFixingPoint - метод  
  
---  
  
Установка координат точки привязки фрагмента, привязанного при помощи переменных привязки

**Пространство имён:** [TFlex.Model.Model2D](N_TFlex_Model_Model2D.md)**Сборка:** TFlexAPI (в TFlexAPI.dll) Версия: 17.1.20.0

```csharp
public void SetFixingPoint(
	int index,
	double x,
	double y
)
```
```vb
Public Sub SetFixingPoint ( 
	index As Integer,
	x As Double,
	y As Double
)
```
```cpp
public:
void SetFixingPoint(
	int index, 
	double x, 
	double y
)
```


#### Параметры

index [Int32](https://learn.microsoft.com/dotnet/api/system.int32)
    Номер точки привязки. Может иметь значение от 1 до 9
x [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата X точки привязки
y [Double](https://learn.microsoft.com/dotnet/api/system.double)
    Координата Y точки привязки

Переменные привязки - переменные в документе фрагмента с имененем x или y и индексом от 1 до 9

#### Ссылки

[Fragment - ](T_TFlex_Model_Model2D_Fragment.md)

[TFlex.Model.Model2D - пространство имён](N_TFlex_Model_Model2D.md)
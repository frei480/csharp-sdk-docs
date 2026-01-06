# Шпаргалка по классам в пространстве имён TFlex.Model.Model2D

## Projection
| Метод | Параметры | Описание |
|---|---|---|
| AddBody(operation) | Operation | Добавление тела |
| SetViewType(type) | ProjectionViewType | Тип вида |
| SetViewWorkplane(plane) | LCSWorkplane | Рабочая плоскость |
| Scale | Parameter | Масштаб |
| SetTiePoint(x,y) | double, double | Точка привязки |

## SimpleDrawingProjection
| Особенность | Описание |
|---|---|
| Наследование | От Projection |
| Использование | Простые виды |
| Настройка | Через LCS и трансформации |

## FreeNode
| Свойство/Конструктор | Тип | Описание |
|---|---|---|
| X | double | Координата X |
| Y | double | Координата Y |
| FreeNode(doc) | Конструктор | Узел в (0,0) |
| FreeNode(doc,x,y) | Конструктор | Узел с координатами |

## LinearDimension
| Метод/Свойство | Тип | Описание |
|---|---|---|
| SetTwoNodes(n1,n2,type) | FreeNode, FreeNode, DimAlignType | Установка узлов |
| SetOffsets(h,v,p,e1,e2,e3) | double?, double?, double?, double, double, double | Отступы |
| ValueType | DimValueType | Тип значения |
| Value | double | Ручное значение |
| Parameter | Parameter | Параметр |

## Перечисления

### DimensionAlignType
- Horizontal - горизонтальный
- Vertical - вертикальный
- Parallel - параллельный
- Aligned - выровненный

### DimensionValueType
- Auto - автоматический
- Manual - ручной
- Parameter - из параметра

## Быстрые примеры

```csharp
// Проекция
SimpleDrawingProjection proj = new SimpleDrawingProjection(doc);
proj.AddBody(operation);
proj.Scale = new Parameter(2.0);
proj.SetTiePoint(100, 100);

// Узлы
FreeNode n1 = new FreeNode(doc, 50, 50);
FreeNode n2 = new FreeNode(doc, 150, 50);

// Размер
LinearDimension dim = new LinearDimension(doc);
dim.SetTwoNodes(n1, n2, DimensionAlignType.Horizontal);
dim.SetOffsets(null, -20, null, 0, null, 0);
dim.ValueType = DimensionValueType.Manual;
dim.Value = 100.0;
```

## Формулы позиционирования

```csharp
// Центр листа
double centerX = (page.Right.Value - page.Left.Value) / 2;
double centerY = (page.Top.Value - page.Bottom.Value) / 2;

// Масштабирование координат
double scaledX = worldX * scale + offsetX;
double scaledY = worldY * scale + offsetY;
```

## Типичные ошибки
- Использование мировых координат без масштабирования
- Неправильные отступы размеров (отрицательные для внутренних)
- Забывание установки ValueType перед Value</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model2D_Cheat_Sheet.md
# Шпаргалка по классам в пространстве имён TFlex.Model.Model3D

## Point3D
| Свойство/Метод | Тип | Описание |
|---|---|---|
| X | double | Координата X |
| Y | double | Координата Y |
| Z | double | Координата Z |
| Point3D() | Конструктор | Создание точки (0,0,0) |
| Point3D(x,y,z) | Конструктор | Создание точки с координатами |

## Direction
| Свойство/Метод | Тип | Описание |
|---|---|---|
| X | double | Компонента X |
| Y | double | Компонента Y |
| Z | double | Компонента Z |
| Length | double | Длина вектора |
| Normalize() | void | Нормализация вектора |
| Direction() | Конструктор | Создание направления (0,0,0) |
| Direction(x,y,z) | Конструктор | Создание направления |

## AffineTransformation
| Метод | Параметры | Описание |
|---|---|---|
| Rotate(axis, angle) | ModelAxis, double | Вращение вокруг оси |
| Translate(x,y,z) | double, double, double | Перенос |
| Scale(x,y,z) | double, double, double | Масштабирование |
| operator* | Point3D/Direction | Применение преобразования |

## LCS
| Свойство/Метод | Тип | Описание |
|---|---|---|
| Geometry.Origin | Point3D | Начало координат |
| Geometry.DirectionX | Direction | Направление оси X |
| Geometry.DirectionY | Direction | Направление оси Y |
| Geometry.DirectionZ | Direction | Направление оси Z |

## Node3D
| Свойство | Тип | Описание |
|---|---|---|
| Position | Point3D | Позиция узла |
| Id | int | Идентификатор |

## LinearDimension3D
| Метод | Параметры | Описание |
|---|---|---|
| SetOrientationPlane(plane) | LCSWorkplane | Установка плоскости |
| SetElements(n1,t1,n2,t2,coords) | Node3D, Dim3DElemType, Node3D, Dim3DElemType, DimUVCoords | Установка элементов |
| SetOffsets(o1,o2,o3) | double, double, double | Установка отступов |

## TransformationGroup
| Метод | Параметры | Описание |
|---|---|---|
| AddMoveTransf(coord, value) | TransCoord, double | Добавление переноса |
| AddRotateTransf(coord, angle) | TransCoord, double | Добавление вращения |
| AddScaleTransf(coord, scale) | TransCoord, double | Добавление масштаба |
| SetLCS(lcs, relative) | LCS, bool | Установка LCS |

## Parameter
| Свойство | Тип | Описание |
|---|---|---|
| Value | double | Численное значение |
| Expression | string | Выражение |

## PointsLCS
| Свойство/Метод | Тип | Описание |
|---|---|---|
| PointToOrigin | Point3D | Точка начала |
| DirectionToAxisX | Direction | Направление X |
| DirectionToAxisY | Direction | Направление Y |
| Name | string | Имя LCS |
| SwitchAroundZ() | void | Переключение вокруг Z |
| SwitchAroundX() | void | Переключение вокруг X |

## LCSWorkplane
| Свойство | Тип | Описание |
|---|---|---|
| LCS | LCS | Связанная LCS |
| Transformations | TransGroup | Группа трансформаций |

## Перечисления

### TransformationCoordinate
- X, Y, Z

### Dimension3DElementType
- Point, Line, Circle, Plane

## Быстрые примеры

```csharp
// Точка
Point3D p = new Point3D(1, 2, 3);

// Направление
Direction d = new Direction(0, 1, 0);
d.Normalize();

// Преобразование
AffineTransformation t = new AffineTransformation();
t.Rotate(new ModelAxis(p, d), Math.PI/2);

// LCS
PointsLCS lcs = new PointsLCS(doc);
lcs.PointToOrigin = p;
lcs.DirectionToAxisX = d;

// Размер
LinearDimension3D dim = new LinearDimension3D(doc);
dim.SetElements(node1, Dim3DElemType.Point, node2, Dim3DElemType.Point, coords);
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D_Cheat_Sheet.md
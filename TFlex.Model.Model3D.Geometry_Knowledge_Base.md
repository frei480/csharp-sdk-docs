# База знаний по классам в пространстве имён TFlex.Model.Model3D.Geometry

## Point3D
**Описание:** Точка в 3D-пространстве.
**Свойства:** X, Y, Z (double)
**Операторы:** +, -, *, /

## Direction
**Описание:** Нормализованный вектор направления.
**Методы:** Normalize(), Length
**Операторы:** *, Dot product

## AffineTransformation
**Описание:** Аффинная трансформация.
**Методы:** Rotate(), Translate(), Scale()
**Оператор:** * (применение к Point3D/Direction)

## Matrix3D
**Описание:** 3D-матрица трансформации.
**Свойства:** Identity
**Операторы:** *

## Quaternion
**Описание:** Кватернион для вращений.
**Методы:** FromAxisAngle(), Rotate()</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Model.Model3D.Geometry_Knowledge_Base.md
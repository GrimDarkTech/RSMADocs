# Настройка физики моделей
[Switch to English](Manual/en/Mechanics/Setting_up_the_physics_of_models.md)

RSMA использует модуль **RSMAMechanicalPart** для моделирования физических взаимодействий.

## Требования
- 3D-модель объекта в формате, [поддерживаемом Unity](https://docs.unity3d.com/Manual/3D-formats.html)
- известная масса объекта
- известные координаты центра масс объекта

## Настройка физики модели на примере рамы мобильного робота
Далее описаны шаги, необходимые для настройки физического моделирования твердых тел. В качестве примера рассмотрена настройка рамы мобильного робота.
## Подготовка объекта
Поместите настраиваемый объект на сцену Unity.
### Настройка положения и ориентации в пространстве

При работе с компонентами RSMA и Unity, например Rigidbody и RSMAHinge, требуется указать точку или направление в локальной системе координат объекта.
Чтобы упростить работу с векторами, рекомендуется настроить положение и поворот объекта перед началом работы с ним.

При импорте 3D-модели в Unity положение и вращение объекта могут быть изменены. Из-за этого модель может быть некорректно ориентирована (рис. 1).\
![1716849507221](/Manual/_images/Setting_up_the_physics_of_models/1716849507221.png)\
Рисунок 1 – Оси направлений изменены, модель ориентированна некорректно

Рекомендуется создать родительский объект для 3D-модели. Для этого щелкните правой кнопкой мыши на объекте в окне "Hierarchy", выберите пункт "Create Empty Parent" (рис. 2) и введите имя нового объекта.\
![1716849814319](/Manual/_images/Setting_up_the_physics_of_models/1716849814319.png)\
Рисунок 2 – Создание родительского объекта

В окне "Hierarchy" выберите дочерний объект и отрегулируйте его вращение и положение с импользованием [инструментов Unity](https://docs.unity3d.com/Manual/PositioningGameObjects.html)
Модель рамы была повернута (рис. 3).\
![1716850197676](/Manual/_images/Setting_up_the_physics_of_models/1716850197676.png)\
Рисунок 3 – Настроенный объект

### Настройка коллайдеров

Коллайдеры определяют физические границы тела. Если у тела нет коллайдера, физический движок будет игнорировать его при обработке столкновений, что приведет к взаимопроникновению тел и некорректному поведению объектов.\

В окне "Hierarchy" выберите родительский объект. Вся дальнейшая настройка будет производиться с родительским объектом (рис. 4).\
![1716850494754](/Manual/_images/Setting_up_the_physics_of_models/1716850494754.png)\
Рисунок 4 – Родительский объект в окне "Hierarchy"

В окне "Inspector" используйте кнопку "Add Component" для поиска и добавления компонента Collider (рис. 5). \
![1716850764808](/Manual/_images/Setting_up_the_physics_of_models/1716850764808.png)\
Рисунок 5 – Добавление компонента Collider\
```Вы можете использовать любой тип 3D-коллайдера или использовать несколько коллайдеров, если потребуется```\
[Узнать больше о коллайдерах](https://docs.unity3d.com/Manual/CollidersOverview.html)

Если коллайдер был успешно добавлен, он отобразится в окне "Inspector" (рис. 6) и отобразится зеленой сеткой вокруг объекта (рис. 7).\
![1716851196960](/Manual/_images/Setting_up_the_physics_of_models/1716851196960.png)\
Рисунок 6 – Настройки компонента Collider в окне "Inspector"\
![1716851501392](/Manual/_images/Setting_up_the_physics_of_models/1716851501392.png)\
Рисунок 7 – Отображение Collider на 3D-модели

Отрегулируйте параметры компонента Collider с использованием настроект в окне "Inspector" (рис. 6).

## Настройка компонента RSMAMechanicalPart
В окне "Inspector" используйте кнопку "Add Component" для поиска и добавления компонента RSMAMechanicalPart (рис. 8).\
![1716851658176](/Manual/_images/Setting_up_the_physics_of_models/1716851658176.png)\
Рисунок 8 – Добавление компонента RSMAMechanicalPart в окне "Inspector"

Если RSMAMechanicalPart был успешно добавлен, он и компонент Rigidbody отобразятся в окне инспектора (рис. 9).\
![1716851803409](/Manual/_images/Setting_up_the_physics_of_models/1716851803409.png)\
Рисунок 9 – Компонент RSMAMechanicalPart в окне "Inspector"

Меню компонента RSMAMechanicalPart содержит следующие поля, используте их для настройки свойств твердого тела:

| Поле | Описание | Тип данных | Принимаемые значения |
|--|--|--|--|
|mass|Масса тела в килограммах|float|от +1,5 x 10e−45 до +3,4 x 10e38|
|centerOfMassPosition|Положение центра масс тела в его локальной системе координат в метрах|Vector3|от ±1,5 x 10e−45 до ±3,4 x 10e38|
|isDrawCenterOfMass|Если значение равно True, то включается отображение положения центра масс тела. Центр масс отображается в виде желтой сферы.|bool|True/False|

При разработке модели рамы в САПР, были определены следующие значения:
- масса рамы - 65 грамм;
- положение центра масс - (0, 2, 0) мм.

Известные значения введены в поля компонента (рис. 10).\
![1716852875787](/Manual/_images/Setting_up_the_physics_of_models/1716852875787.png)\
Рисунок 10 – Настроенный компонент

## Задания

С целью получения опыта настройки физических моделей и улучшения навыков работы с компонентом RSMAMechanicalPart, разработайте:
- модель колеса для мобильной платформы;
- модель рамы мобильной платформы;
- модель звеньев манипулятора (каждое звено - отдельная модель).

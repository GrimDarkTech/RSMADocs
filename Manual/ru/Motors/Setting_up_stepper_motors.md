# Настройка шагового электродвигателя

[Switch to English](Manual/en/Motors/Setting_up_stepper_motors.md)

RSMA использует модуль **StepperMotor** для моделирования работы шаговых электродвигателей.

## Требования

- модель двигателя с настроенной физикой твердого тела
- модель тела, соединенного с валом двигателя (механическая передача, дифференциал, рабочий орган) с настроенными имитационными модулями
- модель драйвера шагового электродвигателя с настроенными имитационными модулями

## Настройка имитационной модели шагового двигателя на примере US17HS4401S

Далее описаны шаги, необходимые для создания и настройки электродвигателя

## Подготовка объектов

Поместите объекты двигателя, драйвера и присоединяемого к двигателю тела на сцену Unity (рис. 1).\
![](/Manual/_images/Setting_up_stepper_motors/Objects.png)\
Рисунок 1 – Настраиваемые объекты

В окне "Hierarchy" выберите присоединяемый объект и отрегулируйте его вращение и положение с импользованием [инструментов Unity](https://docs.unity3d.com/Manual/PositioningGameObjects.html).
В рассматриваемом примере, колесо совмещено с валом электродвигателя (рис. 2).\
![](/Manual/_images/Setting_up_stepper_motors/Placed.png)\
Рисунок 2 – Колесо совмещено с валом двигателя

## Настройка компонента StepperMotor

В окне "Hierarchy" выберите объект двигателя (рис. 3).\
![img](/Manual/_images/Setting_up_stepper_motors/Selected.png)\
Рисунок 3 – Выбран двигатель US17HS4401S

В окне "Inspector" используйте кнопку "Add Component" для поиска и добавления компонента StepperMotor (рис. 4).\
![](/Manual/_images/Setting_up_stepper_motors/AddComponent.png)\
Рисунок 4 – Добавление компонента StepperMotor в окне "Inspector"

Если RSMAMotor2 был успешно добавлен, он отобразится в окне инспектора (рис. 5).\
![](/Manual/_images/Setting_up_stepper_motors/Component.png)\
Рисунок 5 –  Компонент StepperMotor в окне "Inspector"

Меню компонента StepperMotor содержит следующие поля, используте их для настройки:

| Поле           | Описание                                                                                                                                                                                                                                               | Тип                | Значение                           |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- | ------------------------------------------ |
| connectedBody      | Твердое тело, соединенное с валом двигателя                                                                                                                                                                               | UnityEngine.Rigidbody | Ссылка                               |
| motorDriver        | Драйвер, к которому подключен двигатель                                                                                                                                                                                      | StepperDriver         | Ссылка                               |
| motorAxis          | Ось вращения вала двигателя, заданая в его локальной системе координат                                                                                                                             | UnityEngine.Vector3   | Вектор единичной длины |
| isResetMotorAnchor | Если значение равно True, то выполняется сброс привязки оси вращения вала в соответствии с полями motorAnchor и connectedAnchor                                                 | System.Boolean        | True/False                                 |
| motorAnchor        | Координаты точки привязки в локальной системе координат двигателя. Определяет точку, через которую проходит ось вращения вала                      | UnityEngine.Vector3   | от ±1,5 x 10e−45 до ±3,4 x 10e38    |
| connectedAnchor    | Координаты точки привязки в локальной системе координат присоединяемого тела. Определяет точку, через которую проходит ось вращения вала | UnityEngine.Vector3   | от ±1,5 x 10e−45 до ±3,4 x 10e38    |
| holdingTorque      | Момент удержания двигателя в нм                                                                                                                                                                                                     | System.Single         | от ±1,5 x 10e−45 до ±3,4 x 10e38    |
| torque             | Крутящий момент, развиваемый двигателем, в нм                                                                                                                                                                            | System.Single         | от ±1,5 x 10e−45 до ±3,4 x 10e38    |
| stepAngle          | Угол шага двигателя                                                                                                                                                                                                                           | System.Single         | от ±1,5 x 10e−45 до ±3,4 x 10e38    |
| maxAngularVelocity | Максимальное значение угловой скорости для присоединенного тела в радианах в секунду                                                                                                 | System.Single         | от ±1,5 x 10e−45 до ±3,4 x 10e38    |
| isDrawAnchors      | Если значение равно True, положение точек привязок отображается сферами, а ось - линиями                                                                                                  | System.Boolean        | True/False                                 |

### Заполнение поля ConnectedBody

Для заполнения поля connectedBody окне "Hierarchy" найдите присоединяемый объект (рабочий орган, механическая передача, дифференциал), наведите на него курсор, зажмите левую кнопку мыши и перенесите его в поле.

В рассматриваемом примере, объект колеса выбран и помещен в поле (рис. 6).\
![](/Manual/_images/Setting_up_motors/ConnectedBody.png)\
Рисунок 6 – Ссылка на объект колеса

### Заполнение поля MotorDriver

Для заполнения поля motorDriver окне "Hierarchy" найдите объект драйвера шагового электродвигателя, наведите на него курсор, зажмите левую кнопку мыши и перенесите его в поле.

В рассматриваемом примере, двигатель подключен к драйверу L298N (рис. 7).\
![](/Manual/_images/Setting_up_stepper_motors/Driver.png)\
Рисунок 7 – Значение поля motorDriver

### Заполнение поля MotorAxis

Для заполнения поля axis необходимо определить направление оси вращения вала в локальной системе координат двигателя.

Убедитесь, что инструмент перемещения объектов переключен на режим работы в локальных координатах, как показано на рисунке 8.\
![](/Manual/_images/Setting_up_hinge_joints/ToolSettings.png)\
Рисунок 8 – Настройки инструмента позиционирования объектов

В окне "Hierarchy" выберите объект двигателя. Выбранный объект выделится в окне "Scene". На выделенном объекте появится инструмент позиционирования (рис. 9).\
![](/Manual/_images/Setting_up_stepper_motors/Axis.png)\
Рисунок 9 – Инструмент позиционирования на выбранном объекте

Направления стрелок инструмента соотвествуют ориентации локальной системы координат объекта, где:

- синяя стрелка - ось Z (вперед);
- красная стрелка - ось X (вправо);
- зеленая стрелка - ось Y (вверх).

В рассматриваемом примере, ось вращения вала параллельна синей стрелке и направлена в противоположную сторону, что соотвествует оси -Z.
Значение поля Axis - (0, 0, -1) - вектор единичной длины, сонаправленный с осью -Z (рис. 10).\
![](/Manual/_images/Setting_up_stepper_motors/AxisValue.png)\
Рисунок 10 – Значение поля motorAxis

### Настройка точек привязки

Для отключения автоматической настройки точек привязки поставьте галочку в поле isResetAnchor.
Настройка точек привзяки производится с использованием полей MotorAnchor и ConnectedAnchor.

Включите отображение точек привязки, поставив галочку в поле isDrawAnchors. Точки прявзки будут отрисованы в окне "Scene", красная сфера - точка привязки двигателя, зеленая - присоединяемого тела. На рисунке 11 показаны точки электродвигателя и колеса.\
![](/Manual/_images/Setting_up_stepper_motors/Anchors.png)\
Рисунок 11 – Отображение точек привязки двигателя и колеса

Изменяя значение поля MotorAnchor переместите красную сферу в точку, в которой будет расположена ось вращения.
Изменяя значение поля ConnectedAnchor переместите зеленую сферу в точку, через которую будет проходить ось вращения.

После запуска моделирования соединение будет настроено так, что зеленая сфера совпадет с красной (рис. 12).\
![](/Manual/_images/Setting_up_stepper_motors/Setted.png)\
Рисунок 12 – Соединение после запуска моделирования

В рассматриваемом примере, заданы следующие настройки привзяки (рис. 13):\
![](/Manual/_images/Setting_up_stepper_motors/Setted2.png)\
Рисунок 13 – Настройки привязки

После завершения настройки отключите отображение сфер, сняв галочку в поле isDrawAnchors.

### Настройка параметров вращения вала

Задайте величину момента удежания, используя поле HoldingTorque. В рассматриваемом примере, момент удержания - 0.022 нм (рис. 14).\
![](/Manual/_images/Setting_up_stepper_motors/HoldingToque.png)\
Рисунок 14 – Значение поля HoldingTorque

Используйте поле Torque, чтобы задать крутящий момент, развиваемый двигателем. Для модели US17HS4401S, момент - 0.4 нм (рис. 15).\
![](/Manual/_images/Setting_up_stepper_motors/Torque.png)\
Рисунок 15 – Значение поля Torque

Задайте величину шага двигателя (угол, на который поворачивается вал двигателя за один шаг) в градусах. Для этого используйте поле StepAngle.
В примере, угол шага - 1.8 градуса (рис. 16).\
![](/Manual/_images/Setting_up_stepper_motors/Step.png)\
Рисунок 16 – Значение поля StepAngle

Если вы ожидаете скорость вращения вала двигателя выше, чем 523 рад/с. Измените это значение в поле maxAngularVelocity.
Значение по умолчанию - 523.

## Задания

С целью получения опыта настройки шаговых электродвигателей и улучшения навыков работы с компонентом StepperMotor, настройте:

- шаговый двигатель GSMIN 28BYJ-48;
- шаговый двигатель Nema23;
- шаговый двигатель Nema 17 (17HS4401).

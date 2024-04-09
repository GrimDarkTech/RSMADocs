# Команды терминала
[Switch to English](../../../Manual/en/Utilities/TerminalCommands.md)

Команды обрабатываются классом __CommandHandler__ .
Вы можете отправить команду на выполнение через RSMA-API или встроенный RSMA-терминал.  
Каждая команда состоит из имени и аргументов, **разделенных пробелами**.  
Пример команды:  
_команда аргумент1 аргумент2_

## Список доступных команд:

### выключение/shutdown
Завершает процесс RSMA и закрывает приложение
#### Шаблон:
```
shutdown
```

---

### help
Автоматически открывает ссылку на эту страницу и возвращает ссылку на репозиторий с документацией в RSMA
#### Шаблон:
```
help
```

---

### server_start
Запускает встроенный сервер RSMA для подключения клиентов через RSMA-API.
#### Шаблон:
```
server_start
```

---

### server_stop
Останавливает встроенный сервер RSMA и отключает всех клиентов, подключенных через RSMA-API
#### Шаблон:
```
server_stop
```

---

### server_send
Отправляет сообщение клиенту, подключенному к серверу через RSMA-API.
#### Шаблон:
```
server_send client message
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|client|Имя клиента|```server_send Tota UwU```|
|message|Текст сообщения|```server_send Tota Let's_dance```|

---

### scene_load
Загружает сцену по названию сцены
#### Шаблон:
```
scene_load name
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|name|Имя сцены|```scene_load SupremeFlat```|

---

### marker
Создает маркер в указанной точке
#### Шаблон:
```
marker name x y z
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|name|Название маркера. Доступны следующие цвета: Blue, Red, Green|```marker Blue 0 0 0```|
|x|Положение оси X в метрах, в котором появится новый маркер|```marker Red 1,2 0 0```|
|y|Положение оси Y в метрах, в котором появится новый маркер|```marker Red 0 5 0```|
|z|Положение оси Z в метрах, в котором появится новый маркер|```marker Red 0 0 7,3```|

---

### wall
Создает стену с заданными параметрами
#### Шаблон:
```
wall name start_x start_y start_z end_x end_y end_z height width
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|start_x|Положение по оси X в метрах места, где начинается стена|```wall 2 0 0 0 0 1 1 1```|
|start_y|Положение по оси Y в метрах места, где начинается стена|```wall 0 2 0 0 0 1 1 1```|
|start_z|Положение по оси Z в метрах места, где начинается стена|```wall 0 0 2 0 0 1 1 1```|
|end_x|Положение по оси X в метрах места, где заканчивается стена|```wall 0 0 1 2 0 0 1 1```|
|end_y|Положение по оси Y в метрах места, где заканчивается стена|```wall 0 0 1 0 2 0 1 1```|
|end_z|Положение по оси Z в метрах места, где заканчивается стена|```wall 0 0 1 0 0 2 1 1```|
|height|Высота стены в метрах|```wall 0 0 1 0 0 2 1,2 1```|
|width|Толщина стены в метрах|```wall 0 0 1 0 0 2 1 0,5```|

---

### robot
Добавляет робота на сцену
#### Шаблон:
```
robot name x y z rx ry rz
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|name|Имя робота. Доступны: DarkieBot_Altushka, DarkieBot_Skuf, DarkieBot_Kitty|```robot DarkieBot_Altushka 0 0,1 0 0 0 0```|
|x|Положение по оси X в метрах места, где появится новый робот|```robot DarkieBot_Altushka 1 0,1 0 0 0 0```|
|y|Положение по оси Y в метрах места, где появится новый робот|```robot DarkieBot_Altushka 0 0,3 0 0 0 0```|
|z|Положение по оси Z в метрах места, где появится новый робот|```robot DarkieBot_Altushka 0 0,1 4 0 0 0```|
|rx|Угол поворота камеры в градусах, перпендикулярный оси X (тангаж)|```robot DarkieBot_Altushka 0 0,1 0 45 0 0```|
|ry|Угол поворота камеры в градусах, перпендикулярный оси Y (рысканье)|```robot DarkieBot_Altushka 0 0,1 0 0 45 0```|
|rz|Угол поворота камеры в градусах, перпендикулярный оси Z (крен)|```robot DarkieBot_Altushka 0 0,1 0 0 0 45```|

---

### gpio_write
Устанавливает значение вывода порта GPIO
#### Шаблон:
```
gpio_write id port pin value
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор GPIO|```gpio_write 0 PA 1 1```|
|port|Название порта GPIO|```gpio_write 0 PB 3 1```|
|pin|Вывод порта GPIO|```gpio_write 0 PA 4 1```|
|value|Значение, которое должно быть установлено|```gpio_write 0 PA 3 0,5```|

---

### gpio_read
Считывает значение вывода порта GPIO
#### Шаблон:
```
gpio_read id port pin
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор GPIO|```gpio_read 0 PA 1```|
|port|Название порта GPIO|```gpio_read 0 PB 3```|
|pin|Вывод порта GPIO|```gpio_read 0 PA 4```|

---

### drone
Создает новый беспилотник/дрон
#### Шаблон:
```
drone x y z
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|x|Положение по оси X в метрах места, где появится новый дрон|```drone 5 0 0```|
|y|Положение по оси Y в метрах места, где появится новый дрон|```drone 0 8 0```|
|z|Положение по оси Z в метрах места, где появится новый дрон|```drone 0 0 1```|

---

### drone_acceleration
Задает направление и величину ускорения дрона
#### Шаблон:
```
drone_acceleration id x y z
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор дрона. По умолчанию на сцене находится дрон с идентификатором 0|```drone_acceleration 5 0 0 0```|
|x|Величина ускорения в направлении X (право) в м/с ^2|```drone_acceleration 0 1,2 0 0```|
|y|Величина ускорения в направлении Y (верх) в м/с ^2|```drone_acceleration 0 0 -5 0```|
|z|Величина ускорения в направлении Z (перед) в м/с ^2|```drone_acceleration 0 0 0 1,2```|

---

### drone_camera
Поворачивает камеру дрона под заданными углами с заданной плавностью
#### Шаблон:
```
drone_camera id x y z smooth
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор дрона. По умолчанию на сцене находится дрон с идентификатором 0|```drone_camera 5 0 0 0 0,1```|
|x|Угол поворота камеры в градусах, перпендикулярный оси X (тангаж)|```drone_camera 0 1,2 0 0 0,1```|
|y|Угол поворота камеры в градусах, перпендикулярный оси Y (рысканье)|```drone_camera 0 0 -5 0 0,1```|
|z|Угол поворота камеры в градусах, перпендикулярный оси Z (крен)|```drone_camera 0 0 0 1,2 0,1```|
|smooth|Шаг плавного поворота. Чем меньше, тем плавнее. При 1 мгновенный поворот|```drone_camera 0 0 0 0 0,01```|

---

### drone_manual_control
Включает/отключает ручное управление дроном
#### Шаблон:
```
drone_manual_control id mode
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор дрона. По умолчанию на сцене находится дрон с идентификатором 0|```drone_manual_control 0 True```|
|mode|True - включает; False - отключает|```drone_manual_control 0 False```|

---

### drone_move
Управляет дроном с помощью ПИД-регулятора для перемещения в указанную точку
#### Шаблон:
```
drone_move id x y z kp ki kd
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор дрона. По умолчанию на сцене находится дрон с идентификатором 0|```drone_move 0 5 5 15 3 2.113 3.065```|
|x|Положение точки на оси X (право) в метрах|```drone_move 0 0 5 10 3 2.113 1.065```|
|y|Положение точки на оси Y (верх) в метрах|```drone_move 0 0 5 10 3 2.513 4.565```|
|z|Положение точки на оси Z (перед) в метрах|```drone_move 0 5 5 15 0.6 1.55 5```|
|kp|Коэффициент пропорциональности ПИД-регулятора|```drone_move 0 1 1 1 2 0.5 0.5```|
|ki|Интегральный коэффициент ПИД-регулятора;|```drone_move 0 1 1 1 0.5 0.2 0.5```|
|kd|Дифференциальный коэффициент ПИД-регулятора;|```drone_move 0 1 1 1 0.5 0.5 0.9```|

---

### drone_switch_camera
Переключает камеру по идентификатору дрона
#### Шаблон:
```
drone_switch_camera id
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор дрона. По умолчанию на сцене находится дрон с идентификатором 0|```drone_switch_camera 0```|

---

### writer_start
Запускает программу записи (Writer), которая записывает данные о местоположении объекта в CSV-файл
#### Шаблон:
```
writer_start id
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор программы записи. Каждый робот оснащен устройством записи. Идентификатор совпадает с идентификатором робота|```writer_start 0```|

---

### writer_stop
Останавливает запись (Writer) данных о местоположении объекта в CSV-файл
#### Шаблон:
```
writer_stop id
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|id|Идентификатор программы записи. Каждый робот оснащен устройством записи. Идентификатор совпадает с идентификатором робота|```writer_stop 0```|

---

#### template
Описание команды
#### Шаблон:
```
template
```
#### Аргументы:
| Аргумент | Описание | Пример |
|--|--|--|
|argument1|описание к argument1|```Example for argument1```|
|argument2|описание к  argument2|```Example for argument2```|
|argument3|описание к  argument3|```Example for argument3```|
|argument4|описание к  argument4|```Example for argument4```|

---
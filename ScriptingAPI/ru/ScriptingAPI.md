# Документация для разработчиков
[Switch to English](/ScriptingAPI/en/ScriptingAPI.md)

Данный раздел включает следующую информацию о структуре RSMA:
- классы C#
    - описание класса
    - публичные поля класса
    - публичные свойства класса
    - публичные методы класса
    - публичные константы класса
- структуры C#
    - описание структуры
    - публичные поля структуры
    - публичные методы структуры
    - публичные константы класса
- интерфейсы C#
    - описание интерфейса
    - свойства интерфейса
    - методы интерфейса



## Классы RSMA
|Название|Описание|Документация|
|--|--|--|
|RSMAFixed|Соединяет два физических тела, образуя жесткое соединение|[Подробнее..](/ScriptingAPI/ru/Mechanics/RSMAFixed.cs.md)|
|RSMAHinge|Соединяет два физических тела, образуя осевое соединение|[Подробнее..](/ScriptingAPI/ru/Mechanics/RSMAHinge.cs.md)|
|RSMAMechanicalPart|Управляет положением и вращением объекта с помощью физического моделирования|[Подробнее..](/ScriptingAPI/ru/Mechanics/RSMAMechanicalPart.cs.md)|
|RSMAMicrocontroller|Абстрактный класс. Реализует свойства и поведение микроконтроллеров, подобных AVR/STM. Содержит GPIO, главное устройство передачи данных и программу управления|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/RSMAMicrocontroller.cs.md)|
|DefaultMicrocontroller|Реализует свойства и поведение микроконтроллеров, подобных AVR/STM. При включении включает светодиод питания|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/DefaultMicrocontroller.cs.md)|
|RSMAGPIO|Реализует свойства и функциональные возможности GPIO|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/RSMAGPIO.cs.md)|
|GPIOPort|Реализует свойства и функциональные возможности порта GPIO|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/GPIOPort.cs.md)|
|GPIOPin|Реализует свойства и функциональные возможности вывода порта GPIO|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/GPIOPin.cs.md)|
|RSMADataTransferMaster|Реализует свойства и функциональные возможности ведущего устройства в протоколе передачи данных|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/RSMADataTransferMaster.cs.md)|
|RSMADataTransferSlave|Реализует свойства и функциональные возможности ведомого устройства в протоколе передачи данных|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/RSMADataTransferSlave.cs.md)|
|LightSensorScript|Реализует свойства и функциональные возможности датчика освещенности|[Подробнее..](/ScriptingAPI/ru/Electronics/LightSensorScript.cs.md)|
|RSMADisplay|Реализует свойства и функциональные возможности текстового дисплея|[Подробнее..](/ScriptingAPI/ru/Electronics/RSMADisplay.cs.md)|
|Encoder|Имитирует работу абсолютного и инкрементального энкодера со встроенным счетчиком импульсов|[Подробнее..](/ScriptingAPI/ru/Electronics/Encoder.cs.md)|
|RSMALED|Реализует свойства и функциональные возможности светодиода|[Подробнее..](/ScriptingAPI/ru/Electronics/RSMALED.cs.md)|
|RSMAMotorDriver|Реализует свойства и функциональные возможности драйвера электродвигателя|[Подробнее..](/ScriptingAPI/ru/Electronics/RSMAMotorDriver.cs.md)|
|RSMARangeFinderBase|Реализует свойства и функциональные возможности лазерного/ультразвукового дальномера|[Подробнее..](/ScriptingAPI/ru/Electronics/RSMARangeFinderBase.cs.md)|
|Differential|Разлагает входящий поток энергии вращения на два исходящих потока, которые взаимозависимы по своим угловым скоростям|[Подробнее..](/ScriptingAPI/ru/Mechanics/Differential.cs.md)|
|Gearbox|Преобразует входящий поток вращательной энергии в один выходящий поток, изменяя вращающий момент выходного вала и угловую скорость|[Подробнее..](/ScriptingAPI/ru/Mechanics/Gearbox.cs.md)|
|RSMAMotor2|Реализует свойства и функциональные возможности электродвигателя|[Подробнее..](/ScriptingAPI/ru/Motors/RSMAMotor2.cs.md)|
|RSMAServo|Реализует свойства и функциональные возможности сервопривода|[Подробнее..](/ScriptingAPI/ru/Motors/RSMAServo.cs.md)|
|StepperMotor|Реализует свойства и функциональные возможности шагового электродвигателя|[Подробнее..](/ScriptingAPI/ru/Motors/StepperMotor.cs.md)|
|StepperDriver|Реализует свойства и функциональные возможности драйвера шагового электродвигателя|[Подробнее..](/ScriptingAPI/ru/Electronics/StepperDriver.cs.md)|
|OmnidirectionalWheel|Класс для создания и настройки всенаправленных колес|[Подробнее..](/ScriptingAPI/ru/OmnidirectionalWheel.cs.md)|
|LimitSwitch|Реализует свойства и функциональные возможности концевого выключателя|[Подробнее..](/ScriptingAPI/ru/Electronics/LimitSwitch.cs.md)|

## Структуры RSMA
|Название|Описание|Документация|
|--|--|--|
|ConnectedPin|Описывает вывод порта GPIO, к которому подключено устройство|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/ConnectedPin.cs.md)|


## Интерфейсы RSMA

|Название|Описание|Документация|
|--|--|--|
|IMicrocontollerProgram|Реализует поведение и свойства программы микроконтроллера|[Подробнее..](/ScriptingAPI/ru/Electronics/Microcontrollers/MicrocontrollerInterfaces.cs.md)|
|IRotationPowered|Реализует функционал и свойства устройства, приводимого в действие вращательной энергией|[Подробнее..](/ScriptingAPI/ru/Mechanics/RotationPowered.cs.md)|
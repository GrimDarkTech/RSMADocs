# Documentation for developers
[Switch to Russian](/ScriptingAPI/ru/ScriptingAPI.md)

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
|RSMAFixed|Соединяет два физических тела, образуя жесткое соединение|[Подробнее..](/ScriptingAPI/en/Mechanics/RSMAFixed.cs.md)|
|RSMAHinge|Соединяет два физических тела, образуя осевое соединение|[Подробнее..](/ScriptingAPI/en/Mechanics/RSMAHinge.cs.md)|
|RSMAMechanicalPart|Управляет положением и вращением объекта с помощью физического моделирования|[Подробнее..](/ScriptingAPI/en/Mechanics/RSMAMechanicalPart.cs.md)|
|RSMAMicrocontroller|Абстрактный класс. Реализует свойства и поведение микроконтроллеров, подобных AVR/STM. Содержит GPIO, главное устройство передачи данных и программу управления|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/RSMAMicrocontroller.cs.md)|
|DefaultMicrocontroller|Реализует свойства и поведение микроконтроллеров, подобных AVR/STM. При включении включает светодиод питания|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/DefaultMicrocontroller.cs.md)|
|RSMAGPIO|Реализует свойства и функциональные возможности GPIO|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/RSMAGPIO.cs.md)|
|GPIOPort|Реализует свойства и функциональные возможности порта GPIO|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/GPIOPort.cs.md)|
|GPIOPin|Реализует свойства и функциональные возможности вывода порта GPIO|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/GPIOPin.cs.md)|
|RSMADataTransferMaster|Реализует свойства и функциональные возможности ведущего устройства в протоколе передачи данных|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/RSMADataTransferMaster.cs.md)|
|RSMADataTransferSlave|Реализует свойства и функциональные возможности ведомого устройства в протоколе передачи данных|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/RSMADataTransferSlave.cs.md)|
|LightSensorScript|Реализует свойства и функциональные возможности датчика освещенности|[Подробнее..](/ScriptingAPI/en/Electronics/LightSensorScript.cs.md)|
|RSMADisplay|Реализует свойства и функциональные возможности текстового дисплея|[Подробнее..](/ScriptingAPI/en/Electronics/RSMADisplay.cs.md)|
|Encoder|Имитирует работу абсолютного и инкрементального энкодера со встроенным счетчиком импульсов|[Подробнее..](/ScriptingAPI/en/Electronics/Encoder.cs.md)|
|RSMALED|Реализует свойства и функциональные возможности светодиода|[Подробнее..](/ScriptingAPI/en/Electronics/RSMALED.cs.md)|
|RSMAMotorDriver|Реализует свойства и функциональные возможности драйвера электродвигателя|[Подробнее..](/ScriptingAPI/en/Electronics/RSMAMotorDriver.cs.md)|
|RSMARangeFinderBase|Реализует свойства и функциональные возможности лазерного/ультразвукового дальномера|[Подробнее..](/ScriptingAPI/en/Electronics/RSMARangeFinderBase.cs.md)|
|Differential|Разлагает входящий поток энергии вращения на два исходящих потока, которые взаимозависимы по своим угловым скоростям|[Подробнее..](/ScriptingAPI/en/Mechanics/Differential.cs.md)|
|Gearbox|Преобразует входящий поток вращательной энергии в один выходящий поток, изменяя вращающий момент выходного вала и угловую скорость|[Подробнее..](/ScriptingAPI/en/Mechanics/Gearbox.cs.md)|
|RSMAMotor2|Реализует свойства и функциональные возможности электродвигателя|[Подробнее..](/ScriptingAPI/en/Motors/RSMAMotor2.cs.md)|
|RSMAServo|Реализует свойства и функциональные возможности сервопривода|[Подробнее..](/ScriptingAPI/en/Motors/RSMAServo.cs.md)|
|StepperMotor|Реализует свойства и функциональные возможности шагового электродвигателя|[Подробнее..](/ScriptingAPI/en/Motors/StepperMotor.cs.md)|
|StepperDriver|Реализует свойства и функциональные возможности драйвера шагового электродвигателя|[Подробнее..](/ScriptingAPI/en/Electronics/StepperDriver.cs.md)|
|OmnidirectionalWheel|Класс для создания и настройки всенаправленных колес|[Подробнее..](/ScriptingAPI/ru/OmnidirectionalWheel.cs.md)|

## Структуры RSMA
|Название|Описание|Документация|
|--|--|--|
|ConnectedPin|Описывает вывод порта GPIO, к которому подключено устройство|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/ConnectedPin.cs.md)|


## Интерфейсы RSMA

|Название|Описание|Документация|
|--|--|--|
|IMicrocontollerProgram|Реализует поведение и свойства программы микроконтроллера|[Подробнее..](/ScriptingAPI/en/Electronics/Microcontrollers/MicrocontrollerInterfaces.cs.md)|
|IRotationPowered|Реализует функционал и свойства устройства, приводимого в действие вращательной энергией|[Подробнее..](/ScriptingAPI/en/Mechanics/RotationPowered.cs.md)|
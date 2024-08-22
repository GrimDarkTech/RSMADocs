# Настройка микроконтроллеров
[Switch to English](/Manual/en/Electronics/Setting_up_microcontrollers.md)

В RSMA для моделирования работы микроконтроллеров используются четыре компонента:
- DefaultMicrocontroller;
- RSMAGPIO;
- RSMADataTransferMaster;
- IMicrocontollerProgram.

## Требования
- модель объекта микроконтроллера с настроенной физикой твердого тела
- распиновка портов GPIO микроконтроллера

## Настройка микроконтролера на примере платы Arduino Nano
Далее описаны шаги, необходимые для создания микроконтроллера
## Подготовка объектов

Поместите объект микроконтроллера на сцену Unity (рис. 1).\
![](/Manual/_images/Setting_up_microcontrollers/Object.png)\
Рисунок 1 – Настраиваемый объект

## Добавление компонентов

В окне "Hierarchy" выберите объект микроконтроллера (рис. 2).\
![](/Manual/_images/Setting_up_microcontrollers/Selection.png)\
Рисунок 2 – Выбрана плата Arduino Nano

В окне "Inspector" используйте кнопку "Add Component" для поиска и добавления компонента микроконтроллера DefaultMicrocontroller (рис. 3).\
![](/Manual/_images/Setting_up_microcontrollers/AddComponent1.png)\
Рисунок 3 – Добавление компонента DefaultMicrocontroller в окне "Inspector"

Аналогичным образом добавьте компоненты RSMAGPIO и RSMADataTransferMaster (рис. 4).\
![](/Manual/_images/Setting_up_microcontrollers/AddComponent23.png)\
Рисунок 4 – Добавление компонентов RSMAGPIO и RSMADataTransferMaster в окне "Inspector"

Если компоненты были успешно добавлены, они отобразятся в окне инспектора (рис. 5).\
![](/Manual/_images/Setting_up_microcontrollers/Components.png)\
Рисунок 5 –  Компоненты в окне "Inspector"

## Подключение переферийных устройств

Подключите переферийные устройства к микроконтроллеру, задав значения полей GPIO, DataBus и PowerLED.

Для заполнения поля GPIO в окне "Inspector" найдите компонент RSMAGPIO, наведите курсор на его заголовок (рис. 6), зажмите левую кнопку мыши и перенесите его в поле GPIO.\
![](/Manual/_images/Setting_up_microcontrollers/Header.png)\
Рисунок 6 –  Заголовок компонента RSMAGPIO

Заполните поле DataBus, перенеся компонент RSMADataTransferMaster в поле.
Пример заполненных полей представлен на рисунке 7:\
![](/Manual/_images/Setting_up_microcontrollers/GPIO_DataBus.png)\
Рисунок 7 –  Заполненные поля GPIO и DataBus

Перед заполнением поля PowerLED необходимо настроить моделирование светодиода.
В окне "Hierarchy" найдите (создайте) и выберите объект светодиода (рис. 8).\
![](/Manual/_images/Setting_up_microcontrollers/LedSelected.png)\
Рисунок 8 – Выбрана светодиодная панель на модели микрокотноллера

В окне "Inspector" используйте кнопку "Add Component" для поиска и добавления компонента микроконтроллера RSMALED (рис. 9).\
![](/Manual/_images/Setting_up_microcontrollers/AddLed.png)\
Рисунок 9 – Добавление компонента DefaultMicrocontroller в окне "Inspector"

Если компонент был успешно добавлен, он и компонент Light отобразятся в окне инспектора (рис. 10).\
![](/Manual/_images/Setting_up_microcontrollers/LedAdded.png)\
Рисунок 10 –  Компоненты RSMALED и Light в окне "Inspector"

Измените радиус освещения светодиода, установив в компоненте Light значение поля Range равным 0.1.
При необходимости измените цвет света, используя поле Color. Для светодиода из примера выбран красный цвет (рис. 11).\
![](/Manual/_images/Setting_up_microcontrollers/Light.png)\
Рисунок 11 –  Настройки компонента Light

Укажите модель корпуса светодиода, используя поле ColorBody. Для этого в окне "Hierarchy" наведите курсор на необохидимый объект, зажмите левую кнопку мыши и перенесите его в поле. Если не задать значение для ColorBody, при запуске моделирования будет выполнен автоматический поиск модели на объекте светодиода.\

В рассматриваемом примере, значение поля ColorBody не задано так, как компонент находится на объекте с моделью светодиода.

Укажите цвет света светодиода в поле Color. Для светодиода из примера выбран красный цвет.\

В окне "Hierarchy" выберите объект микроконтроллера и задайте значение поля PowerLED. Для этого в окне "Hierarchy" наведите курсор на ранее настроенный объект светодиода, зажмите левую кнопку мыши и перенесите его в поле.\

Все переферийные устройства подключены (рис. 12).\
![](/Manual/_images/Setting_up_microcontrollers/MicrocontrollerSetted.png)\
Рисунок 12 –  Настроенный компонент DefaultMicrocontroller

## Настройка GPIO

Компонент GPIO в RSMA содержит список портов, каждый порт содержит список выводов. Изначально список протов пуст.

Разверните поле Ports и добавьте новые порты, нажимая на значок "+" (рис. 13).\
![](/Manual/_images/Setting_up_microcontrollers/AddPort.png)\
Рисунок 13 – Добавление портов GPIO

В поле Name укажите имя порта, в каждый порт добавьте список выводов, нажимая на значок "+".

В Arduino Nano GPIO состоит из 3 портов: PB, PC, PD.
Порт PB содержит 6 выводов, PC - 7, PD - 8. Порты настроены в соотвествии с распиновкой (рис. 14).\
![](/Manual/_images/Setting_up_microcontrollers/PortsSetted.png)\
Рисунок 14 – Порты GPIO Arduino Nano

Настройте выводы каждого порта, введя имена выводов в поле Name (рис. 15). Остальные настройки - по умолчанию.\
![](/Manual/_images/Setting_up_microcontrollers/PinsSetted.png)\
Рисунок 14 – Выводы портов GPIO

## Подключение внешних устройств к шине передачи данных

Для передачи данных в RSMA используется компонент RSMADataTransferMaster. RSMADataTransferMaster поддерживает работу только с экземплярами классов унаследованных от RSMADataTransferSlave. Далее прведен алгоритм подключения устройств для передачи данных на примере текстового дисплея.

Добавьте подключаемое устройство на сцену Unity.

В окне "Hierarchy" выберите объект микроконтроллера. В копоненте RSMADataTransferMaster разверните поле DataBus и добавьте новое устройство, нажав на значок "+" (рис. 16).\
![](/Manual/_images/Setting_up_microcontrollers/AddDevice.png)\
Рисунок 16 – Добавление нового устройства

В окне "Hierarchy" наведите курсор на подключаемое устройство, зажмите левую кнопку мыши и перенесите его в новое поле списка DataBus.
В рассматриваемом примере, к Arduino Nano подключен текстовый дисплей (рис. 17).\
![](/Manual/_images/Setting_up_microcontrollers/DeviceConnected.png)\
Рисунок 17 – Подключение дисплея

## Написание программы для микроконтроллера

Для разработки программ микроконтроллеров в RSMA существует интерфейс IMicrocontollerProgram.
Рекомендуется создать отдельную папку для хранения программ. В RSMA программы хранятся в дирректории ```Assets/Scripts/Microcontroller/Programs```

Для создания нового файла программы нажмите правой кнопкой мыши в окне "Project", во всплывающем окне, в пункте "RSMA" выберите "Create Firmware File".\
![](/Manual/_images/Setting_up_microcontrollers/CreateFirmware.png)\
Рисунок 18 – Вызов меню создания программ

В открывшемся окне "Firmware Creator" (рис. 19), в поле FirmwareName укажите имя файла программы микроконтроллера. Рекомендуется использовать только буквы латинского алфавита и цифры, не используйте пробелы.\
![](/Manual/_images/Setting_up_microcontrollers/FirmwareCreator.png)\
Рисунок 19 – Окно "Firmware Creator"

Нажмите кнопку "Create Firmware", чтобы создать новый файл программы.

Откройте файл редактором кода. Содержимое созданного файла представлено ниже:
``` C#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;
public class ManualProgram : MonoBehaviour, IMicrocontollerProgram
{
    public RSMAGPIO GPIO { get; set; }

    public  RSMADataTransferMaster dataBus { get; set; }
    public IEnumerator MainProgramm()
    {
        yield return new WaitForSeconds(0.1f);
    }
}
```
Метод MainProgramm() является точкой входа в программу микроконтроллера.

Чтобы выполнить программу, добавьте ее как компонент к объекту микроконтроллера. Для этого в окне "Hierarchy" выберите объект микроконтроллера.
В окне "Inspector" используйте кнопку "Add Component" для поиска и добавления файла программы. В качестве примера была создана и добавлена программа "ManualProgram" (рис. 20).\
![](/Manual/_images/Setting_up_microcontrollers/ManualProgram.png)\
Рисунок 20 – Добавление компонента ManualProgram в окне "Inspector"

## Задания

С целью получения опыта настройки микроконтроллеров и улучшения навыков работы с компонентами DefaultMicrocontroller, RSMAGPIO и RSMADataTransferMaster, соберите:
- Arduino Mega;
- Arduino Uno;
- ESP32.

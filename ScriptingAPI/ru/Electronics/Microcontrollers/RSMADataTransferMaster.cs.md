# RSMADataTransferMaster
[switch to English](/ScriptingAPI/en/Electronics/Microcontrollers/RSMADataTransferMaster.cs.md)

 Реализует свойства и функциональность главного устройства в протоколе передачи данных

## Поля
| Поле | Описание | Тип |
|--|--|--|
|dataBus|     Список устройств, подключенных к главному устройству по шине передачи данных|System.Collections.Generic.List`1[RSMADataTransferSlave]|
|data|     Запрашивает имя целевого устройства|System.String|

## Методы
### SendData
     Отправляет данные на целевое устройство
#### Объявление:
    public virtual void SendData(int targetAddress)
#### Возвращает:

### ReciveData
     Получает данные с целевого устройства
#### Объявление:
    public virtual void ReciveData(int targetAddress)
#### Возвращает:

### Request
     Запрашивает имя целевого устройства
#### Объявление:
    public virtual void RequestName(int targetAddress)
#### Возвращает:

### RequestName
     Запрашивает имя целевого устройства
#### Объявление:
    public virtual void RequestName(int targetAddress)
#### Возвращает:

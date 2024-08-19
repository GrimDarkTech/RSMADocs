# RSMADataTransferSlave
[switch to English](/ScriptingAPI/en/Electronics/Microcontrollers/RSMADataTransferSlave.cs.md)

 Реализует свойства и функциональность подчиненного устройства в протоколе передачи данных

## Методы
### SetDeviceName
     Задает имя устройства
#### Объявление:
    public  void SetDeviceName(string deviceName)
#### Возвращает:

### GetDeviceName
     Получает имя устройства
#### Объявление:
    public string GetDeviceName()
#### Возвращает:
     Имя устройства
### SendData
     Возвращает данные
#### Declaration:
    public virtual string SendData()
#### Возвращает:
     Данные
### SendName
     Возвращает имя устройства
#### Объявление:
    public virtual string SendName()
#### Returns:
     
### OnRequest
     Вызывается по запросу главного устройства
#### Объявление:
    public virtual void OnRequest()
#### Возвращает:

### ReciveData
     Получает данные из шины данных
#### Объявление:
    public virtual void ReciveData(string recivedData)
#### Возвращает:

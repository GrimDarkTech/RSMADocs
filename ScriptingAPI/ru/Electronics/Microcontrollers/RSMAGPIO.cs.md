# RSMAGPIO
[switch to English](/ScriptingAPI/en/Electronics/Microcontrollers/RSMAGPIO.cs.md)

 Реализует свойства и функциональность GPIO
 
## Константы
| Поле | Описание | Тип | Значение |
|--|--|--|--|
|High|     Постоянное значение вывода порта GPIO в активном состоянии|System.Single|1|
|Low|     Постоянное значение вывода порта GPIO в неактивном состоянии|System.Single|0|

## Методы
### GetPortList
     Возвращает список портов GPIO
#### Объявление:
    public List<GPIOPort> GetPortList()
#### Возвращает:
     Список портов
### WritePin
     Переключает выходное значение вывода порта GPIO
#### Объявление:
    public void WritePin(string portName, int pinIndex, float value)
#### Возвращает:

### WritePin
     Переключает выходное значение вывода порта GPIO
#### Объявление:
    public void WritePin(string portName, int pinIndex, float value)
#### Возвращает:

### WritePin
     Переключает выходное значение вывода порта GPIO
#### Объявление:
    public void WritePin(string portName, int pinIndex, float value)
#### Возвращает:

### WritePin
     Переключает выходное значение вывода порта GPIO
#### Объявление:
    public void WritePin(string portName, int pinIndex, float value)
#### Возвращает:

### GetPin
     Gets GPIO port pin object by ConnectedPin enum
#### Объявление:
    public GPIOPin GetPin(ConnectedPin connectedPin)
#### Возвращает:
     Возвращает ссылку на вывод GPIO, если он существует, иначе возвращает null
### GetPin
     Gets GPIO port pin object by ConnectedPin enum
#### Объявление:
    public GPIOPin GetPin(ConnectedPin connectedPin)
#### Возвращает:
     Возвращает ссылку на вывод GPIO, если он существует, иначе возвращает null
### ResetAll
     Устанавливает значения контактов портов GPIO по умолчанию
#### Объявление:
    public void ResetAll()
#### Возвращает:

### TurnOffAll
     Устанавливает значения контактов портов GPIO равными 0
#### Объявление:
    public void TurnOffAll()
#### Возвращает:

### ReadPin
     Считать входное значение контакта порта GPIO 
#### Объявление:
    public float ReadPin(string portName, int pinIndex)
#### Возвращает:
     Возвращает float значение контакта порта GPIO
### ReadPin
     Считать входное значение контакта порта GPIO
#### Объявление:
    public float ReadPin(string portName, int pinIndex)
#### Возвращает:
     Возвращает float значение контакта порта GPIO
### ReadPin
     Считать входное значение контакта порта GPIO 
#### Объявление:
    public float ReadPin(string portName, int pinIndex)
#### Возвращает:
     Возвращает float значение контакта порта GPIO
### ReadPin
     Считать входное значение контакта порта GPIO
#### Объявление:
    public float ReadPin(string portName, int pinIndex)
#### Возвращает:
     Возвращает float значение контакта порта GPIO

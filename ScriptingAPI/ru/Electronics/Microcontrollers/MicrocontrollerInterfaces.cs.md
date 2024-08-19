# IMicrocontollerProgram
[switch to English](/ScriptingAPI/en/Electronics/Microcontrollers/MicrocontrollerInterfaces.cs.md)

Интерфейс. Реализует поведение и свойства программы микроконтроллера.

## Поля
| Поле | Описание | Тип |
|--|--|--|
|GPIO|GPIO микроконтроллера|RSMAGPIO|
|dataBus| шина данных микроконтроллера для протоколов передачи данных|RSMADataTransferMaster|

## Методы

### MainProgramm
Точка входа в программу микроконтроллера
#### Объявление:
public IEnumerator MainProgramm()
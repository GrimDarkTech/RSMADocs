# IMicrocontollerProgram
[switch to Russian](/ScriptingAPI/ru/Electronics/Microcontrollers/MicrocontrollerInterfaces.cs.md)

Interface. Implements behavior and properties of microcontroller program

## Properties
| Field | Description | Type |
|--|--|--|
|GPIO|Microcontroller GPIO|RSMAGPIO|
|dataBus|Microcontroller databus for data transfer protocols|RSMADataTransferMaster|

## Methods

### MainProgramm
Entry point to microcontroller program
#### Declaration:
public IEnumerator MainProgramm()
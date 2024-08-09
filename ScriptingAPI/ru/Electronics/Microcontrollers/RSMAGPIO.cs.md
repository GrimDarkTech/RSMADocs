# RSMAGPIO
[switch to Russian](/ScriptingAPI/ru/Electronics/Microcontrollers/RSMAGPIO.cs.md)

 Implements properties and functionality of GPIO

## Constants
| Field | Description | Type | Value |
|--|--|--|--|
|High|     Constant value of GPIO port pin in active state|System.Single|1|
|Low|     Constant value of GPIO port pin in inactive state|System.Single|0|

## Methods
### GetPortList
     Returns GPIO ports list
#### Declaration:
    public List<GPIOPort> GetPortList()
#### Returns:
     List of ports
### WritePin
     Toggles output value of GPIO port pin
#### Declaration:
    public void WritePin(string portName, int pinIndex, float value)
#### Returns:

### WritePin
     Toggles output value of GPIO port pin
#### Declaration:
    public void WritePin(string portName, int pinIndex, float value)
#### Returns:

### WritePin
     Toggles output value of GPIO port pin
#### Declaration:
    public void WritePin(string portName, int pinIndex, float value)
#### Returns:

### WritePin
     Toggles output value of GPIO port pin
#### Declaration:
    public void WritePin(string portName, int pinIndex, float value)
#### Returns:

### GetPin
     Gets GPIO port pin object by ConnectedPin enum
#### Declaration:
    public GPIOPin GetPin(ConnectedPin connectedPin)
#### Returns:
     Returns GPIOPin ref if it exists, else returns null
### GetPin
     Gets GPIO port pin object by ConnectedPin enum
#### Declaration:
    public GPIOPin GetPin(ConnectedPin connectedPin)
#### Returns:
     Returns GPIOPin ref if it exists, else returns null
### ResetAll
     Sets default GPIO ports pins values
#### Declaration:
    public void ResetAll()
#### Returns:

### TurnOffAll
     Sets GPIO ports pins values to 0
#### Declaration:
    public void TurnOffAll()
#### Returns:

### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value
### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value
### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value
### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value

# RSMALED
[switch to Russian](/ScriptingAPI/ru/Electronics/RSMALED.cs.md)

 Implements properties and functionality of Light Emitting Diode 

## Fields
| Field | Description | Type |
|--|--|--|
|colorBody|     LED body. Object which model will change color when the LED is turned on/off. If the value is not set, the component will try to find it automatically on the object to which it is attached|UnityEngine.Renderer|
|color|     LED color |UnityEngine.Color|
|connectedPin|     GPIO port pin which LED is connected|ConnectedPin|
|connectMicrocontroller|     GPIO which LED is connected|RSMAGPIO|

## Methods
### SetMode
     Sets LED mode
#### Declaration:
    public void SetMode(ushort mode)
#### Returns:
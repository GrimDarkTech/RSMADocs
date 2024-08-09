# LightSensorScript
[switch to Russian](/ScriptingAPI/ru/Electronics/LightSensorScript.cs.md)

 Implements properties and functionality of light sensor

## Fields
| Field | Description | Type |
|--|--|--|
|lightIntensity|Light intensity value determined by sensor|System.Single|
|lightCoefficient|Scale factor for calculating light intensity|System.Single|

## Methods
### SendData
     Sends light intensity data via a data transfer protocol
#### Declaration:
    public override string SendData()
#### Returns:
     Returns light intensity value
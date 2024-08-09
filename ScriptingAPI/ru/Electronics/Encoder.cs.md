# Encoder
[switch to Russian](/ScriptingAPI/ru/Electronics/Encoder.cs.md)

 Simulates the operation of an absolute and incremental encoder with a built-in pulse counter.

## Fields
| Field | Description | Type |
|--|--|--|
|type|     Type of device being modeled|RSMA.EncoderType|
|resolution|     The resolution of the encoder. Number of pulses per revolution|System.Int32|
|connectedBody|     Body connected to encoder shaft|UnityEngine.GameObject|
|axis|     Represents the encoder axis, emanating from origin|UnityEngine.Vector3|

## Methods
### SendData
     Sends the number of pulses measured by the encoder
#### Declaration:
    public override string SendData()
#### Returns:
     Number of pulses measured by the encoder counter

# RSMARangeFinderBase
[switch to Russian](/ScriptingAPI/ru/Electronics/RSMARangeFinderBase.cs.md)

 Implements properties and functionality of rangefinder

## Fields
| Field | Description | Type |
|--|--|--|
|maxRange|     Maximum range that can be measured by rangefinder|System.Single|
|angle||System.Single|
|numberOfRays|     Number of rays casted on angle|System.Int32|

## Methods
### SendData
     Sends measured range via datatransfer protocol
#### Declaration:
    public override string SendData()
#### Returns:
     Returns measured range coverted to string
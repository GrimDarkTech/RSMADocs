# RSMARangeFinderBase
[switch to Russian](/ScriptingAPI/ru/Electronics/RSMARangeFinderBase.cs.md)

 Implements properties and functionality of rangefinder

## Fields
| Field | Description | Type |
|--|--|--|
|maxRange|     Maximum range that can be measured by rangefinder|System.Single|
|angle|Viewing angle of the rangefinder. The angle lies in the zx plane (horizontal) , z axis (forward) - is the bisector of the angle|System.Single|
|numberOfRays|     Number of rays casted on angle|System.Int32|
|isDrawRays|If True, draws rays of rangefinder|System.Boolean|
## Methods
### SendData
     Sends measured range via datatransfer protocol
#### Declaration:
    public override string SendData()
#### Returns:
     Returns measured range coverted to string
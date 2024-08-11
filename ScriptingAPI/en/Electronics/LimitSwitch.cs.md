# LimitSwitch
[switch to Russian](/ScriptingAPI/ru/Electronics/LimitSwitch.cs.md)

 Implements the properties and functionality of the limit switch

## Fields
| Field | Description | Type |
|--|--|--|
|stock|Switch stock|UnityEngine.GameObject|
|stockAxis|The axis of movement of the stock in local coordinates|CoordinateAxis|
|stockFreeStroke|Determines the free stroke of the stock|System.Single|
|springStiffness|Switch spring stiffness|System.Single|
|springDamper|Switch damper|System.Single|
|maxForce|The maximum force a spring can exert|System.Single|
|triggerDistance|The distance between the anchors, which activates switch|System.Single|
|bodyAnchor|Represents the anchor for switch body|UnityEngine.Vector3|
|stockAnchor|Represents the anchor for switch stock|UnityEngine.Vector3|
|isDrawAnchors|If True, draws anchors position with spheres|System.Boolean|

## Methods
### SendData
     Sends switch state via datatransfer protocol
#### Declaration:
    public override string SendData()
#### Returns:
     Returns 1, if Switch is active(pressed), else returns 0

# RSMAServo
[switch to Russian](/ScriptingAPI/ru/Motors/RSMAServo.cs.md)

Implements properties and functionality of servo motor

## Fields
| Field | Description | Type |
|--|--|--|
|connectedBody|     Body used as a motor rotor|UnityEngine.Rigidbody|
|axis||UnityEngine.Vector3|
|microcontroller|     Microcontroller GPIO connected to servo|RSMAGPIO|
|connectedPin|     Microcontroller GPIO port pin connected to servo|ConnectedPin|
|isUseLimits|     If True, servo has limits|System.Boolean|
|limits|     Angles, that limits servo shaft rotation|UnityEngine.Vector2|
|torque|     Maximum torque value|System.Single|
|damper|     Damping factor|System.Single|
|isResetAnchor|     If True, resets the Anchor according to the anchor and connectedAnchor fields|System.Boolean|
|anchor||UnityEngine.Vector3|
|connectedAnchor|     Represents the anchor position for connected body|UnityEngine.Vector3|
|isDrawAnchors|     If True, draws anchors position with spheres and axis with lines|System.Boolean|

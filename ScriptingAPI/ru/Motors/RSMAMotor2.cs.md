# RSMAMotor2
[switch to Russian](/ScriptingAPI/ru/Motors/RSMAMotor2.cs.md)

 Implements properties and functionality of electric motor

## Fields
| Field | Description | Type |
|--|--|--|
|mechanicalCharacteristics|     A curve describing the mechanical characteristic of an electric motor (the dependence of the torque on the angular velocity of the shaft)|UnityEngine.AnimationCurve|
|connectedBody|     Body used as a motor rotor|UnityEngine.GameObject|
|motorDriver|     Driver connected to motor|RSMAMotorDriver|
|motorAxis|     Represents the motor axis, emanating from origin|UnityEngine.Vector3|
|isResetMotorAnchor|     If True, resets the Anchor according to the anchor and connectedAnchor fields|System.Boolean|
|motorAnchor|     Represents the Motor Anchor|UnityEngine.Vector3|
|connectedAnchor|     Represents the anchor for connected body|UnityEngine.Vector3|
|brakingFactor|     Braking factor|System.Single|
|outputTorque|     Value of the torque of rotation of the output shaft|System.Single|
|maxAngularVelocity|     Max value of angular velocity for connected body|System.Single|
|isDrawAnchors|     If True, draws anchors position with spheres and axis with lines|System.Boolean|

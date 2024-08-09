# StepperMotor
[switch to Russian](/ScriptingAPI/ru/Motors/StepperMotor.cs.md)

 Implements properties and functionality of stepper motor

## Fields
| Field | Description | Type |
|--|--|--|
|connectedBody|     Body used as a motor rotor|UnityEngine.GameObject|
|motorDriver|     Driver connected to motor|StepperDriver|
|motorAxis|     Represents the motor axis, emanating from origin|UnityEngine.Vector3|
|isResetMotorAnchor|     Resets MotorAnchor with startMotorAnchor|System.Boolean|
|motorAnchor|     Represents the Motor Anchor|UnityEngine.Vector3|
|connectedAnchor|     Represents the anchor for connected body|UnityEngine.Vector3|
|holdingTorque|     Holding torque|System.Single|
|torque|     Rotation torque|System.Single|
|stepAngle|     Step angle|System.Single|
|maxAngularVelocity|     The maximum value of the angular velocity of rotation of the body attached to the motor shaft. 523 radians per second - default|System.Single|
|isDrawAnchors|     If True draws anchors|System.Boolean|

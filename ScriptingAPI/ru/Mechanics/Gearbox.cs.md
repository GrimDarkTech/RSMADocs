# Gearbox
[switch to English](/ScriptingAPI/en/Mechanics/Gearbox.cs.md)

Converts the incoming flow of rotational energy into one outgoing flow by changing the torque of the output shaft and the angular velocity

## Fields
| Field | Description | Type |
|--|--|--|
|ratio|     Gear ratio of the gearbox|System.Single|
|connectedBody|     Body connected to output of the gearbox|UnityEngine.Rigidbody|
|brakingFactor|     Braking factor|System.Single|
|gearboxAxis|     Axis of output of the gearbox|UnityEngine.Vector3|
|isResetAnchor|     If True, resets anchors with anchor and connectedAnchor|System.Boolean|
|anchor|The coordinates of the anchor point in the local coordinate system of the object. Defines the point through which the axis of rotation passes|UnityEngine.Vector3|
|connectedAnchor|The coordinates of the anchor point in the local coordinate system of the connected body. Defines the point through which the axis of rotation passes|UnityEngine.Vector3|
|maxAngularVelocity|     Max value of angular velocity for connected body|System.Single|
|isDrawAnchors|     If True, draws anchors position with spheres and axis with lines|System.Boolean|
|outputTorque|     Value of the torque of rotation of the output shaft|UnityEngine.Vector3|
## Properties
| Property | Description | Type |
|--|--|--|
|rigidbody|     Body of gearbox|UnityEngine.Rigidbody|
|inputAngularVelocity|     Value of the angular velocity of rotation of the input shaft|System.Single|
|inputTorque|     Value of the torque of rotation of the input shaft|System.Single|
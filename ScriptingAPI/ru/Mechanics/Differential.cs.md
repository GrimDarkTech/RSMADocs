# Differential
[switch to Russian](/ScriptingAPI/ru/Mechanics/Differential.cs.md)

 Decomposes  incoming flow of rotational power into two outgoing flows that are interdependent in their angular velocities

## Fields
| Field | Description | Type |
|--|--|--|
|rightGearRatio|     Gear ratio of the right output of the differential|System.Single|
|leftGearRatio|     Gear ratio of the left output of the differential|System.Single|
|rightConnectedBody|     Body connected to right output of the gearbox|UnityEngine.Rigidbody|
|rightAxis|     Axis of output of the gearbox|UnityEngine.Vector3|
|isResetRightAnchor|     Resets right anchor setting|System.Boolean|
|rightAnchor|     Right anchor position|UnityEngine.Vector3|
|rightConnectedAnchor|     Right connected body anchor position|UnityEngine.Vector3|
|leftConnectedBody|     Body connected to right output of the gearbox|UnityEngine.Rigidbody|
|leftAxis|     Axis of output of the gearbox|UnityEngine.Vector3|
|isResetLeftAnchor|     Resets left anchor setting|System.Boolean|
|leftAnchor|     Left anchor position|UnityEngine.Vector3|
|leftConnectedAnchor|     Left connected body anchor position|UnityEngine.Vector3|
|brakingFactor|     Braking factor|System.Single|
|maxAngularVelocity|     Max value of angular velocity for connected bodies|System.Single|
|isDrawAnchors|     If True, draws anchors position with spheres and axis with lines|System.Boolean|
|outputTorque|     Value of the torque of rotation of the output shafts|UnityEngine.Vector3|
## Properties
| Property | Description | Type |
|--|--|--|
|rigidbody|Rigidbody of differetial|UnityEngine.Rigidbody|
|inputAngularVelocity|     Value of the angular velocity of rotation of the input shaft|System.Single|
|inputTorque|     Value of the torque of rotation of the input shaft|System.Single|

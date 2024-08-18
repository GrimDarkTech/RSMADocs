# RSMAHinge
[switch to Russian](/ScriptingAPI/ru/Mechanics/RSMAHinge.cs.md)

Simulates the behavior of the axial connection. The hinge joint is used to simulate the interaction of two rigid bodies

## Fields
| Field | Description | Type |
|--|--|--|
|connectedBody|Body connected to hinge joint|UnityEngine.Rigidbody|
|axis|The axis of rotation, set in the local coordinate system of the object|UnityEngine.Vector3|
|isResetAnchor|If True, resets the Anchor according to the anchor and connectedAnchor fields|System.Boolean|
|anchor|The coordinates of the anchor point in the local coordinate system of the object. Defines the point through which the axis of rotation passes|UnityEngine.Vector3|
|connectedAnchor|The coordinates of the anchor point in the local coordinate system of the connected body. Defines the point through which the axis of rotation passes|UnityEngine.Vector3|
|isDrawAnchors|If True, draws anchors position with spheres and axis with lines|System.Boolean|

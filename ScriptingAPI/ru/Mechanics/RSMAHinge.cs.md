# RSMAHinge
[switch to Russian](/ScriptingAPI/ru/Mechanics/RSMAHinge.cs.md)

Simulates the behavior of the axial connection. The hinge joint is used to simulate the interaction of two rigid bodies

## Fields
| Field | Description | Type |
|--|--|--|
|connectedBody|     Body connected to hinge joint|UnityEngine.Rigidbody|
|axis||UnityEngine.Vector3|
|isResetAnchor|     If True, resets the Anchor according to the anchor and connectedAnchor fields|System.Boolean|
|anchor||UnityEngine.Vector3|
|connectedAnchor|     Represents the anchor for connected body|UnityEngine.Vector3|
|isDrawAnchors|     If True, draws anchors position with spheres and axis with lines|System.Boolean|

# OmnidirectionalWheel
[switch to Russian](/ScriptingAPI/ru/Mechanics/OmnidirectionalWheel.cs.md)

 Class for creating and configuring omnidirectional wheels

## Fields
| Field | Description | Type |
|--|--|--|
|wheel|Wheel object used as the basis for an omnidirectional wheel|UnityEngine.GameObject|
|wheelRotation|Rotation of the wheel object|UnityEngine.Quaternion|
|roller|Roller object used to form an omnidirectional wheel|UnityEngine.GameObject|
|rollerCount|The number of rollers mounted on the wheel|System.Int32|
|installationRadius|The radius of installation of the rollers|System.Single|
|additionalRollerRotation|Additional rotation of the rollers object|UnityEngine.Quaternion|
|wheelPlane|The plane of rotation of the wheel in the local coordinate system|CoordinatePlane|
|rollerAngle|The angle of inclination of the rollers relative to the circumference of the wheel|System.Single|
|rollerRotationAxis|The axis relative to which the roller is rotated to the wheel plane|CoordinateAxis|
|rollerHingeAxis|The axis of rotation of the roller|CoordinateAxis|

## Methods
### FormWheel
    Creates a wheel with the specified parameters on the attached object
#### Declaration:
    public void FormWheel()
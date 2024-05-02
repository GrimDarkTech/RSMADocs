# RSMAEncoder
[switch to API](../../../Documentation/ScriptingAPI/en/RSMAEncoder.cs.md)



## Fields
| Field | Description | Type |
|--|--|--|
|EncoderTypeObj|     Defines the type of encoder used in the simulation|EncoderType|
|EncoderRangeType| limits of the rotation|EncoderRangeType|
|AxisDirection|     Determines which side the encoder will be located relative to the motor|AxisEnum|
|OutPut|     Determines how much data the encoder transmits over the data transmitter|EncoderOutput|
|AutoAxis|     to the motor     Automatic determination of the axis from which the encoder will be connected |System.Boolean|
|Distance|     the distance can be negative and positive     At what distance from the object the encoder will be located|System.Single|
|EncoderResolution|     shaft or bore.      output by the encoder during one 360 degree revolution of the encoder      Encoder resolution is the number of pulses per revolution (PPR) or bits |System.Single|
|Shaft|     the object of the shaft that will spin together with the motor|UnityEngine.GameObject|
|Motor|     Motor of the object under study|UnityEngine.HingeJoint|
## Properties
| Property | Description | Type |
|--|--|--|
|useGUILayout||System.Boolean|
|runInEditMode||System.Boolean|
|enabled||System.Boolean|
|isActiveAndEnabled||System.Boolean|
|transform||UnityEngine.Transform|
|gameObject||UnityEngine.GameObject|
|tag||System.String|
|rigidbody||UnityEngine.Component|
|rigidbody2D||UnityEngine.Component|
|camera||UnityEngine.Component|
|light||UnityEngine.Component|
|animation||UnityEngine.Component|
|constantForce||UnityEngine.Component|
|renderer||UnityEngine.Component|
|audio||UnityEngine.Component|
|networkView||UnityEngine.Component|
|collider||UnityEngine.Component|
|collider2D||UnityEngine.Component|
|hingeJoint||UnityEngine.Component|
|particleSystem||UnityEngine.Component|
|name||System.String|
|hideFlags||UnityEngine.HideFlags|
## Methods
### GetVelocity
     Get the speed of rotation of the shaft in degrees per second
#### Declaration:
    public float GetVelocity()
#### Returns:

### GetSide
     2 - left side     1 - right side     0 - no side     Get the direction of the shaft
#### Declaration:
    public int GetSide()
#### Returns:

### GetHZ
     Get the rotation frequency of the encoder shaft
#### Declaration:
    public string GetHZ()
#### Returns:
     
### GetMeasureAngle
     updates the data     Get the calculated step angle with which the encoder 
#### Declaration:
    public string GetMeasureAngle()
#### Returns:

### GetAngle
     depends on the type of encoder     Get the angle of rotation of the encoder shaft, which 
#### Declaration:
    public float GetAngle()
#### Returns:
     
### SendData

#### Declaration:

#### Returns:

### SetDeviceName

#### Declaration:

#### Returns:

### GetDeviceName

#### Declaration:

#### Returns:

### SendName

#### Declaration:

#### Returns:

### OnRequest

#### Declaration:

#### Returns:

### ReciveData

#### Declaration:

#### Returns:

### IsInvoking

#### Declaration:

#### Returns:

### CancelInvoke

#### Declaration:

#### Returns:

### Invoke

#### Declaration:

#### Returns:

### InvokeRepeating

#### Declaration:

#### Returns:

### CancelInvoke

#### Declaration:

#### Returns:

### IsInvoking

#### Declaration:

#### Returns:

### StartCoroutine

#### Declaration:

#### Returns:

### StartCoroutine

#### Declaration:

#### Returns:

### StartCoroutine

#### Declaration:

#### Returns:

### StartCoroutine_Auto

#### Declaration:

#### Returns:

### StopCoroutine

#### Declaration:

#### Returns:

### StopCoroutine

#### Declaration:

#### Returns:

### StopCoroutine

#### Declaration:

#### Returns:

### StopAllCoroutines

#### Declaration:

#### Returns:

### get_useGUILayout

#### Declaration:

#### Returns:

### set_useGUILayout

#### Declaration:

#### Returns:

### get_runInEditMode

#### Declaration:

#### Returns:

### set_runInEditMode

#### Declaration:

#### Returns:

### get_enabled

#### Declaration:

#### Returns:

### set_enabled

#### Declaration:

#### Returns:

### get_isActiveAndEnabled

#### Declaration:

#### Returns:

### get_transform

#### Declaration:

#### Returns:

### get_gameObject

#### Declaration:

#### Returns:

### GetComponent

#### Declaration:

#### Returns:

### GetComponent

#### Declaration:

#### Returns:

### TryGetComponent

#### Declaration:

#### Returns:

### TryGetComponent

#### Declaration:

#### Returns:

### GetComponent

#### Declaration:

#### Returns:

### GetComponentInChildren

#### Declaration:

#### Returns:

### GetComponentInChildren

#### Declaration:

#### Returns:

### GetComponentInChildren

#### Declaration:

#### Returns:

### GetComponentInChildren

#### Declaration:

#### Returns:

### GetComponentsInChildren

#### Declaration:

#### Returns:

### GetComponentsInChildren

#### Declaration:

#### Returns:

### GetComponentsInChildren

#### Declaration:

#### Returns:

### GetComponentsInChildren

#### Declaration:

#### Returns:

### GetComponentsInChildren

#### Declaration:

#### Returns:

### GetComponentsInChildren

#### Declaration:

#### Returns:

### GetComponentInParent

#### Declaration:

#### Returns:

### GetComponentInParent

#### Declaration:

#### Returns:

### GetComponentInParent

#### Declaration:

#### Returns:

### GetComponentInParent

#### Declaration:

#### Returns:

### GetComponentsInParent

#### Declaration:

#### Returns:

### GetComponentsInParent

#### Declaration:

#### Returns:

### GetComponentsInParent

#### Declaration:

#### Returns:

### GetComponentsInParent

#### Declaration:

#### Returns:

### GetComponentsInParent

#### Declaration:

#### Returns:

### GetComponents

#### Declaration:

#### Returns:

### GetComponents

#### Declaration:

#### Returns:

### GetComponents

#### Declaration:

#### Returns:

### get_tag

#### Declaration:

#### Returns:

### set_tag

#### Declaration:

#### Returns:

### GetComponents

#### Declaration:

#### Returns:

### CompareTag

#### Declaration:

#### Returns:

### SendMessageUpwards

#### Declaration:

#### Returns:

### SendMessageUpwards

#### Declaration:

#### Returns:

### SendMessageUpwards

#### Declaration:

#### Returns:

### SendMessageUpwards

#### Declaration:

#### Returns:

### SendMessage

#### Declaration:

#### Returns:

### SendMessage

#### Declaration:

#### Returns:

### SendMessage

#### Declaration:

#### Returns:

### SendMessage

#### Declaration:

#### Returns:

### BroadcastMessage

#### Declaration:

#### Returns:

### BroadcastMessage

#### Declaration:

#### Returns:

### BroadcastMessage

#### Declaration:

#### Returns:

### BroadcastMessage

#### Declaration:

#### Returns:

### get_rigidbody

#### Declaration:

#### Returns:

### get_rigidbody2D

#### Declaration:

#### Returns:

### get_camera

#### Declaration:

#### Returns:

### get_light

#### Declaration:

#### Returns:

### get_animation

#### Declaration:

#### Returns:

### get_constantForce

#### Declaration:

#### Returns:

### get_renderer

#### Declaration:

#### Returns:

### get_audio

#### Declaration:

#### Returns:

### get_networkView

#### Declaration:

#### Returns:

### get_collider

#### Declaration:

#### Returns:

### get_collider2D

#### Declaration:

#### Returns:

### get_hingeJoint

#### Declaration:

#### Returns:

### get_particleSystem

#### Declaration:

#### Returns:

### GetInstanceID

#### Declaration:

#### Returns:

### GetHashCode

#### Declaration:

#### Returns:

### Equals

#### Declaration:

#### Returns:

### get_name

#### Declaration:

#### Returns:

### set_name

#### Declaration:

#### Returns:

### get_hideFlags

#### Declaration:

#### Returns:

### set_hideFlags

#### Declaration:

#### Returns:

### ToString

#### Declaration:

#### Returns:

### GetType

#### Declaration:

#### Returns:

# RSMAEncoderEditor
[switch to API](../../../Documentation/ScriptingAPI/en/RSMAEncoder.cs.md)



## Properties
| Property | Description | Type |
|--|--|--|
|target||UnityEngine.Object|
|targets||UnityEngine.Object[]|
|serializedObject||UnityEditor.SerializedObject|
|name||System.String|
|hideFlags||UnityEngine.HideFlags|
## Methods
### OnInspectorGUI

#### Declaration:

#### Returns:

### get_target

#### Declaration:

#### Returns:

### set_target

#### Declaration:

#### Returns:

### get_targets

#### Declaration:

#### Returns:

### get_serializedObject

#### Declaration:

#### Returns:

### DrawDefaultInspector

#### Declaration:

#### Returns:

### Repaint

#### Declaration:

#### Returns:

### CreateInspectorGUI

#### Declaration:

#### Returns:

### RequiresConstantRepaint

#### Declaration:

#### Returns:

### DrawHeader

#### Declaration:

#### Returns:

### HasPreviewGUI

#### Declaration:

#### Returns:

### GetPreviewTitle

#### Declaration:

#### Returns:

### RenderStaticPreview

#### Declaration:

#### Returns:

### OnPreviewGUI

#### Declaration:

#### Returns:

### OnInteractivePreviewGUI

#### Declaration:

#### Returns:

### OnPreviewSettings

#### Declaration:

#### Returns:

### GetInfoString

#### Declaration:

#### Returns:

### DrawPreview

#### Declaration:

#### Returns:

### ReloadPreviewInstances

#### Declaration:

#### Returns:

### UseDefaultMargins

#### Declaration:

#### Returns:

### Initialize

#### Declaration:

#### Returns:

### Cleanup

#### Declaration:

#### Returns:

### MoveNextTarget

#### Declaration:

#### Returns:

### ResetTarget

#### Declaration:

#### Returns:

### SetDirty

#### Declaration:

#### Returns:

### GetInstanceID

#### Declaration:

#### Returns:

### GetHashCode

#### Declaration:

#### Returns:

### Equals

#### Declaration:

#### Returns:

### get_name

#### Declaration:

#### Returns:

### set_name

#### Declaration:

#### Returns:

### get_hideFlags

#### Declaration:

#### Returns:

### set_hideFlags

#### Declaration:

#### Returns:

### ToString

#### Declaration:

#### Returns:

### GetType

#### Declaration:

#### Returns:


# RSMAGPIO
[switch to API](../../../Documentation/ScriptingAPI/en/RSMAGPIO.cs.md)

 Implements properties and functionality of GPIO

## Fields
| Field | Description | Type |
|--|--|--|
|High|     Constant value of GPIO port pin in active state|System.Single|
|Low|     Constant value of GPIO port pin in inactive state|System.Single|
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
### GetPortList
     Returns GPIO ports list
#### Declaration:
    public List<GPIOPort> GetPortList()
#### Returns:
     List of ports
### WritePin

#### Declaration:

#### Returns:

### WritePin

#### Declaration:

#### Returns:

### WritePin

#### Declaration:

#### Returns:

### WritePin

#### Declaration:

#### Returns:

### GetPin
     Gets GPIO port pin object by ConnectedPin enum
#### Declaration:
    public GPIOPin GetPin(ConnectedPin connectedPin)
#### Returns:
     Returns GPIOPin ref if it exists, else returns null
### GetPin
     Gets GPIO port pin object by ConnectedPin enum
#### Declaration:
    public GPIOPin GetPin(ConnectedPin connectedPin)
#### Returns:
     Returns GPIOPin ref if it exists, else returns null
### ResetAll
     Sets default GPIO ports pins values
#### Declaration:
    public void ResetAll()
#### Returns:

### TurnOffAll
     Sets GPIO ports pins values to 0
#### Declaration:
    public void TurnOffAll()
#### Returns:

### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value
### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value
### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value
### ReadPin
     Read input value of GPIO port pin 
#### Declaration:
    public float ReadPin(string portName, int pinIndex)
#### Returns:
     Returns float GPIO port pin value
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


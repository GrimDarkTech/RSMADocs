# Switch
[switch to API](../../../Documentation/ScriptingAPI/en/Switch.cs.md)



## Fields
| Field | Description | Type |
|--|--|--|
|TypeEnum||SwitchTypeEnum|
|MechState|     The state of closure or opening of an electrical circuit.|System.Boolean|
|ButtonDamper|     Resistance to movement due to viscous friction.|System.Single|
|ButtonSpring|     The force returns to its previous shape after compression or stretching.|System.Single|
|MaxLength|     Maximum button pressing distance|System.Single|
|HorButtonSlider|     of the button, which is displayed as a percentage.     the activation point is within the initial position to the limit position |System.Single|
|AngularDamper|     Resistance to movement due to viscous friction for angle.|System.Single|
|AngularSpring|     the angular view.     The force returns to its previous shape after compression or stretching in |System.Single|
|MinAngle|     The minimum angle at which the lever can turn.|System.Single|
|MaxAngle|     The maximum angle at which the lever can turn|System.Single|
|HorLeverRollerSlider|     of the lever, which is displayed as a percentage.     the activation point is within the initial angle to the limit angle |System.Single|
|Joint|     Erases all settings of configurable joint of lever and sets new ones|UnityEngine.ConfigurableJoint|
|AnchorPos|     Fulcrum of configurable joint.|UnityEngine.Vector3|
|Vector|     Direction of the axis of rotation.|UnityEngine.Vector3|
|SizeGizmoSphere|     The size of the gizmo that is displayed in the unity user interface.|System.Single|
|DoCalculations|     An event that performs calculations depending on the type of limit switch.|System.Action|
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
### SwitchOn
     It is triggered when the limit switch switches to the on state
#### Declaration:
    public void SwitchOn()
#### Returns:

### SwitchOff
     It is triggered when the limit switch switches to the off state
#### Declaration:
    public void SwitchOff()
#### Returns:

### ResetJoint
     Erases all settings of configurable joint of lever and sets new ones
#### Declaration:
    public void ResetJoint()
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

# SwitchEditor
[switch to API](../../../Documentation/ScriptingAPI/en/Switch.cs.md)



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


# RSMADisplay
[switch to Russian](/ScriptingAPI/ru/Electronics/RSMADisplay.cs.md)

 Implements properties and functionality of text display

## Fields
| Field | Description | Type |
|--|--|--|
|text|     TextMesh component used to display text|TMPro.TextMeshPro|
|fontSize|     Font size in millimeters|System.Single|
|fontColor|     Font color in RGB|UnityEngine.Color|
|characterSpacing|     Character spacing in em|System.Single|
|lineSpacing|     Line spacing in em|System.Single|
|lowerLeftAnchor|     Lower left corner of the display|UnityEngine.Vector3|
|upperRightAnchor|     Upper right corner of the display|UnityEngine.Vector3|
|isDrawAnchors|     If True, displays the position of the anchors|System.Boolean|

## Methods
### ReciveData
Sets display's text
#### Declaration:
public override void ReciveData(string recivedData)
#### Returns:
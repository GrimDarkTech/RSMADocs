# Terminal Commands

Commands are handled by the __CommandHandler__ class.
You can send a command for execution via the RSMA-API or the built-in RSMA terminal.  
Each command consists of a name and arguments separated by spaces.  
Command example:  
_command argument1 argument2_

## List of available commands:

### shutdown
Terminates the RSMA process and closes the application

---

### help
Automatically opens a link to this page and returns a link to the repository with documentation to RSMA

---

### server
Manages the built-in RSMA server for connecting clients via the RSMA API.
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|start|Starts the RSMA server. Uses port 7777|```server start```|
|stop|Stops the server|```server stop```|
|send|Sends a message to the connected client by the client's name|```server send Tod Hey_Tod!```|

---

### drone
Creates a new drone
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|x|The X-axis position in meters where the new drone will appear|```drone 5 0 0```|
|y|The Y-axis position in meters where the new drone will appear|```drone 0 8 0```|
|z|The Z-axis position in meters where the new drone will appear|```drone 0 0 1```|

---

### droneMove
Sets the direction and magnitude of the drone thrust and yaw
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The drone's ID. By default, there is a drone with ID 0 on the stage|```droneMove 5 0 0 0 45```|
|x|The magnitude of the acceleration in the direction X (right) in m/s ^2|```droneMove 0 1,2 0 0 0```|
|y|The magnitude of the acceleration in the direction Y (up) in m/s ^2|```droneMove 0 0 -5 0 0```|
|z|The magnitude of the acceleration in the direction Z (forward) in m/s ^2|```droneMove 0 0 0 1,2 0```|
|yaw|Drone yaw. It is set relative to the direction of the cardinal directions|```droneMove 0 0 0 0 45```|

---

### droneCamera
Rotates the drone's camera at preset angles with a preset smoothness
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The drone's ID. By default, there is a drone with ID 0 on the stage|```droneCamera 5 0 0 0 0,1```|
|x|The angle of rotation of the camera in degrees perpendicular to the X axis (pitch)|```droneMove 0 1,2 0 0 0```|
|y|The angle of rotation of the camera in degrees perpendicular to the Y axis (yaw)|```droneMove 0 0 -5 0 0```|
|z|The angle of rotation of the camera in degrees perpendicular to the Z axis (roll)|```droneMove 0 0 0 1,2 0```|
|smooth|The step of a smooth turn. The smaller, the smoother. At 1 instant turn|```droneMove 0 0 0 0 0,01```|

---

### template
Description of the command.
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|argument1|Description of the argument1|```Example for argument1```|
|argument2|Description of the argument2|```Example for argument2```|
|argument3|Description of the argument3|```Example for argument3```|
|argument4|Description of the argument4|```Example for argument4```|

---
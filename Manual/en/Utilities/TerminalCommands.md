# Terminal Commands
[Switch to Russian](../../../Manual/ru/Utilities/TerminalCommands.md)

Commands are handled by the __CommandHandler__ class.
You can send a command for execution via the RSMA-API or the built-in RSMA terminal.  
Each command consists of a name and arguments **separated by spaces**.  
Command example:  
_command argument1 argument2_

## List of available commands:

### shutdown
Terminates the RSMA process and closes the application
#### Template:
```
shutdown
```

---

### help
Automatically opens a link to this page and returns a link to the repository with documentation to RSMA
#### Template:
```
help
```

---

### server_start
Starts the built-in RSMA server for connecting clients via the RSMA API.
#### Template:
```
server_start
```

---

### server_stop
Stops the built-in RSMA server for connecting clients via the RSMA API.
#### Template:
```
server_stop
```

---

### server_send
Sends a message to the client connected to the server via the RSMA API.
#### Template:
```
server_send client message
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|client|Client name|```server_send Tota UwU```|
|message|Message text|```server_send Tota Let's_dance```|

---

### scene_load
Loads a scene by the name of the scene
#### Template:
```
scene_load name
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|name|Scene name|```scene_load SupremeFlat```|

---

### marker
Creates a marker at the specified point
#### Template:
```
marker name x y z
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|name|The name of the marker. Available in: Blue, Red, Green|```marker Blue 0 0 0```|
|x|The X-axis position in meters where the new marker will appear|```marker Red 1,2 0 0```|
|y|The Y-axis position in meters where the new marker will appear|```marker Red 0 5 0```|
|z|The Z-axis position in meters where the new marker will appear|```marker Red 0 0 7,3```|

---

### wall
Creates a wall with the specified parameters
#### Template:
```
wall name start_x start_y start_z end_x end_y end_z height width
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|start_x|The X-axis position in meters where does the wall begins|```wall 2 0 0 0 0 1 1 1```|
|start_y|The Y-axis position in meters where does the wall begins|```wall 0 2 0 0 0 1 1 1```|
|start_z|The Z-axis position in meters where does the wall begins|```wall 0 0 2 0 0 1 1 1```|
|end_x|The X-axis position in meters where does the wall ends|```wall 0 0 1 2 0 0 1 1```|
|end_y|The Y-axis position in meters where does the wall ends|```wall 0 0 1 0 2 0 1 1```|
|end_z|The Z-axis position in meters where does the wall ends|```wall 0 0 1 0 0 2 1 1```|
|height|Wall height in meters|```wall 0 0 1 0 0 2 1,2 1```|
|width|Wall width in meters|```wall 0 0 1 0 0 2 1 0,5```|

---

### robot
Adds a robot to the scene
#### Template:
```
robot name x y z rx ry rz
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|name|The name of the robot. Available: DarkieBot_Altushka, DarkieBot_Skuf, DarkieBot_Kitty|```robot DarkieBot_Altushka 0 0,1 0 0 0 0```|
|x|The X-axis position in meters where the new robot will appear|```robot DarkieBot_Altushka 1 0,1 0 0 0 0```|
|y|The Y-axis position in meters where the new robot will appear|```robot DarkieBot_Altushka 0 0,3 0 0 0 0```|
|z|The Z-axis position in meters where the new robot will appear|```robot DarkieBot_Altushka 0 0,1 4 0 0 0```|
|rx|The angle of rotation of the camera in degrees perpendicular to the X axis (pitch)|```robot DarkieBot_Altushka 0 0,1 0 45 0 0```|
|ry|The angle of rotation of the camera in degrees perpendicular to the Y axis (yaw)|```robot DarkieBot_Altushka 0 0,1 0 0 45 0```|
|rz|The angle of rotation of the camera in degrees perpendicular to the Z axis (roll)|```robot DarkieBot_Altushka 0 0,1 0 0 0 45```|

---

### gpio_write
Sets the value of the GPIO port pin
#### Template:
```
gpio_write id port pin value
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The GPIO's ID|```gpio_write 0 PA 1 1```|
|port|GPIO port name|```gpio_write 0 PB 3 1```|
|pin|GPIO port pin|```gpio_write 0 PA 4 1```|
|value|The value to be set|```gpio_write 0 PA 3 0,5```|

---

### gpio_read
Reads the value of the GPIO port pin
#### Template:
```
gpio_read id port pin
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The GPIO's ID|```gpio_read 0 PA 1```|
|port|GPIO port name|```gpio_read 0 PB 3```|
|pin|GPIO port pin|```gpio_read 0 PA 4```|

---

### drone
Creates a new drone
#### Template:
```
drone x y z
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|x|The X-axis position in meters where the new drone will appear|```drone 5 0 0```|
|y|The Y-axis position in meters where the new drone will appear|```drone 0 8 0```|
|z|The Z-axis position in meters where the new drone will appear|```drone 0 0 1```|

---

### drone_acceleration
Sets the direction and magnitude of the drone acceleration
#### Template:
```
drone_acceleration id x y z
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The drone's ID. By default, there is a drone with ID 0 on the stage|```drone_acceleration 5 0 0 0```|
|x|The magnitude of the acceleration in the direction X (right) in m/s ^2|```drone_acceleration 0 1,2 0 0```|
|y|The magnitude of the acceleration in the direction Y (up) in m/s ^2|```drone_acceleration 0 0 -5 0```|
|z|The magnitude of the acceleration in the direction Z (forward) in m/s ^2|```drone_acceleration 0 0 0 1,2```|

---

### drone_camera
Rotates the drone's camera at preset angles with a preset smoothness
#### Template:
```
drone_camera id x y z smooth
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The drone's ID. By default, there is a drone with ID 0 on the stage|```drone_camera 5 0 0 0 0,1```|
|x|The angle of rotation of the camera in degrees perpendicular to the X axis (pitch)|```drone_camera 0 1,2 0 0 0,1```|
|y|The angle of rotation of the camera in degrees perpendicular to the Y axis (yaw)|```drone_camera 0 0 -5 0 0,1```|
|z|The angle of rotation of the camera in degrees perpendicular to the Z axis (roll)|```drone_camera 0 0 0 1,2 0,1```|
|smooth|The step of a smooth turn. The smaller, the smoother. At 1 instant turn|```drone_camera 0 0 0 0 0,01```|

---

### drone_manual_control
Enables/disables manual drone control
#### Template:
```
drone_manual_control id mode
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The drone's ID. By default, there is a drone with ID 0 on the stage|```drone_manual_control 0 True```|
|mode|True - enables; False - disables|```drone_manual_control 0 False```|

---

### drone_move
Controls the drone using a PID controller to move to the specified point
#### Template:
```
drone_move id x y z kp ki kd
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The drone's ID. By default, there is a drone with ID 0 on the stage|```drone_move 0 5 5 15 3 2.113 3.065```|
|x|The position of the point on the X axis (right) in m|```drone_move 0 0 5 10 3 2.113 1.065```|
|y|The position of the point on the Y axis (up) in m|```drone_move 0 0 5 10 3 2.513 4.565```|
|z|The position of the point on the Z axis (forward) in m|```drone_move 0 5 5 15 0.6 1.55 5```|
|kp|Proportional coefficient of the PID controller|```drone_move 0 1 1 1 2 0.5 0.5```|
|ki| Integral coefficient of the PID controller;|```drone_move 0 1 1 1 0.5 0.2 0.5```|
|kd|Differential coefficient of the PID controller;|```drone_move 0 1 1 1 0.5 0.5 0.9```|

---

### drone_switch_camera
Switches the camera by drone ID
#### Template:
```
drone_switch_camera id
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The drone's ID. By default, there is a drone with ID 0 on the stage|```drone_switch_camera 0```|

---

### writer_start
Starts a Writer that writes data about the object's position to a CSV file
#### Template:
```
writer_start id
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The ID of the writer. Each robot is equipped with a writer. The ID matches the robot's ID|```writer_start 0```|

---

### writer_stop
Stops the writer writing data about the object's position to a CSV file
#### Template:
```
writer_stop id
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|id|The ID of the writer. Each robot is equipped with a writer. The ID matches the robot's ID|```writer_stop 0```|

---

### template
Description of the command.
#### Template:
```
template
```
#### Arguments:
| Argument | Description | Example |
|--|--|--|
|argument1|Description of the argument1|```Example for argument1```|
|argument2|Description of the argument2|```Example for argument2```|
|argument3|Description of the argument3|```Example for argument3```|
|argument4|Description of the argument4|```Example for argument4```|

---
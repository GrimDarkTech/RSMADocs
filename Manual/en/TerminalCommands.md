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
# SocketClient
[switch to API](../../../Documentation/ScriptingAPI/en/SocketClient.cs.md)

 �lass implements the behavior of a socket client. Uses to connect to server, send and receive messages

## Fields
| Field | Description | Type |
|--|--|--|
|serverIP|     Server IP address|System.String|
|serverPort|     Port binded by the server|System.Int32|
|clientName|     Name of client|System.String|
|isConnected|     True if client connected to server|System.Boolean|
## Methods
### OnConnected
     Called when client connected to server
#### Declaration:
    public virtual void OnConnected() { }
#### Returns:

### OnDisconnected
     Called when client disconnected to server
#### Declaration:
    public virtual void OnDisconnected() { }
#### Returns:

### OnMessageDelivered
     Called when message delivered to server
#### Declaration:
    public virtual void OnMessageDelivered() { }
#### Returns:

### OnMessageRecived
     Called when recived message from server
#### Declaration:
    public virtual void OnMessageRecived(string message) { }
#### Returns:

### ConnectAsync
     Connects client to server
#### Declaration:
    public async void ConnectAsync()
#### Returns:

### SendMessageAsync
     Sends message to server
#### Declaration:
    public async void SendMessageAsync(string message)
#### Returns:

### DisconnectAsync
     Disconnects cleint from server
#### Declaration:
    public async void DisconnectAsync()
#### Returns:

### Equals

#### Declaration:

#### Returns:

### GetHashCode

#### Declaration:

#### Returns:

### GetType

#### Declaration:

#### Returns:

### ToString

#### Declaration:

#### Returns:


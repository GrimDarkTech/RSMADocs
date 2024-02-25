# SocketServer
[switch to API](../../../Documentation/ScriptingAPI/en/SocketServer.cs.md)

 Сlass implements the behavior of a socket server. Uses to connect clients, send and receive messages

## Fields
| Field | Description | Type |
|--|--|--|
|serverIP|     Server IP address|System.String|
|serverPort|     Port binded by the server|System.Int32|
|cliensNames|     Clients names|System.Collections.Generic.List`1[System.String]|
|isStarted|     True if server started|System.Boolean|
## Methods
### OnStarted
     Called on server ready to listen clients
#### Declaration:
    public virtual void OnStarted() { }
#### Returns:

### OnStopped
     Called on server stopped
#### Declaration:
    public virtual void OnStopped() { }
#### Returns:

### OnClientConnected
     Called when new client connected
#### Declaration:
    public virtual void OnClientConnected(string clientName) { }
#### Returns:

### OnClientDisconnected
     Called when client disconnected
#### Declaration:
    public virtual void OnClientDisconnected(string clientName) { }
#### Returns:

### OnMessageDelivered
     Called when message delivered to client
#### Declaration:
    public virtual void OnMessageDelivered(string clientName) { }
#### Returns:

### OnMessageRecived
     Called when message recived
#### Declaration:
    public virtual void OnMessageRecived(string clientName, string message) { }
#### Returns:

### Run
     Starts server
#### Declaration:
    public void Run()
#### Returns:

### Stop
     Stops server
#### Declaration:
    public void Stop()
#### Returns:

### SendMessageToClientAsync
     Sends message to client
#### Declaration:
    public async void SendMessageToClientAsync(string clientName, string message)
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


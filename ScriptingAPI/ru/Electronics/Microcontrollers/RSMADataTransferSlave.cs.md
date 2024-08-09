# RSMADataTransferSlave
[switch to Russian](/ScriptingAPI/ru/Electronics/Microcontrollers/RSMADataTransferSlave.cs.md)

 Implements properties and functionality of slave device in data transfer protocol

## Methods
### SetDeviceName
     Sets device name
#### Declaration:
    public  void SetDeviceName(string deviceName)
#### Returns:

### GetDeviceName
     Gets device name
#### Declaration:
    public string GetDeviceName()
#### Returns:
     Device name
### SendData
     Returns data
#### Declaration:
    public virtual string SendData()
#### Returns:
     Data
### SendName
     Returns device name
#### Declaration:
    public virtual string SendName()
#### Returns:
     
### OnRequest
     Called when master device requests
#### Declaration:
    public virtual void OnRequest()
#### Returns:

### ReciveData
     Recives data from data bus
#### Declaration:
    public virtual void ReciveData(string recivedData)
#### Returns:

# RSMADataTransferMaster
[switch to Russian](/ScriptingAPI/ru/Electronics/Microcontrollers/RSMADataTransferMaster.cs.md)

 Implements properties and functionality of master device in data transfer protocol

## Fields
| Field | Description | Type |
|--|--|--|
|dataBus|     List of devices connected to master device via the data bus|System.Collections.Generic.List`1[RSMADataTransferSlave]|
|data|     Requests name of target device|System.String|

## Methods
### SendData
     Sends data to target device
#### Declaration:
    public virtual void SendData(int targetAddress)
#### Returns:

### ReciveData
     Recives data from target device
#### Declaration:
    public virtual void ReciveData(int targetAddress)
#### Returns:

### Request
     Requests name of target device
#### Declaration:
    public virtual void RequestName(int targetAddress)
#### Returns:

### RequestName
     Requests name of target device
#### Declaration:
    public virtual void RequestName(int targetAddress)
#### Returns:

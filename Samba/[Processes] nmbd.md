# NetBIOS Name Service Daemon Overview

nmbd is the NetBIOS name server daemon that handles NetBIOS over IP (NetBT or NBT) name service requests from SMB/CIFS clients

* Allows client machines to locate resources by NetBIOS names on a network
* Supports network browsing by participating in elections for local master browser roles and maintaining browse lists for discovering shares and printers

<br>

# nmbd Ports

| Port Number | Description |
| --- | --- | 
| 137/UDP | Name service |
| 138/UDP | Datagram service |
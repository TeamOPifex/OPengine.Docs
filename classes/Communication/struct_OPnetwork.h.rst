OPnetwork.h
=========

OPnetworkPacketRaw
----------------
- OPchar* Buffer
- i32 Length
OPnetworkPacket
----------------
- OPnetworkPacketRaw* RawPacket
- i32 ClientId
- OPchar* Message
OPneworkData
----------------
- fd_set master
- fd_set read_fds
- i32 fdmax
- i32 clientIndex
-  peer_addr
-  peer_host
-  peer_port
OPneworkClientData
----------------
- i32 fd
OPnetwork
----------------
- i32 ConnectSocket
-  ConnectionType
-  ConnectionProtocol
- OPneworkData Data
- void() receive
- void() connected
- void() disconnected
Globals
----------------
Functions
----------------
- OPnetwork* OPnetworkCreate (  networkType,  protocol )
- i32 OPnetworkClientConnect ( OPnetwork* network, OPchar* address, OPchar* port )
- i32 OPnetworkServerStart ( OPnetwork* network, OPchar* port )
- OPnetwork* OPnetworkAcceptClient ( OPnetwork* network )
- i32 OPnetworkReceive ( OPnetwork* network, void* state )
- i32 OPnetworkSend ( OPnetwork* network, i8* data, i32 size )
- i32 OPnetworkShutdown ( OPnetwork* network )
- void OPnetworkDestroy ( OPnetwork* network )
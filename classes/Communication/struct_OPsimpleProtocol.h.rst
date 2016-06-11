OPsimpleProtocol.h
=========

OPprotocolSimpleMessage
----------------
- i32 TimeStamp
- i32 DataLength
- i8* Data
OPnetworkProtocolSimple
----------------
- OPnetwork* Network
-  LastReceived
- i32 LastSent
- void() Receive
Globals
----------------
Functions
----------------
- OPnetworkProtocolSimple* OPnetworkProtocolSimpleCreate (  networkType )
- i32 OPnetworkProtocolSimpleReceive ( OPnetworkProtocolSimple* protocol, void() receive )
- i32 OPnetworkProtocolSimpleSend ( OPnetworkProtocolSimple* protocol, OPtimer* timer, i8* data, i32 size )
- void OPnetworkProtocolSimpleDestroy ( OPnetworkProtocolSimple* protocol )
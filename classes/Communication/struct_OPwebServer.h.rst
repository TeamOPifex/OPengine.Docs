OPwebServer.h
=========

OPwebServer
----------------
- mg_server* Server
- void() Receive
- OPhashMap* WebSocketKeys
- ui32 messageCount
-  messages
OPWebServerHandlerContainer
----------------
- void() handler
- void* param
Globals
----------------
Functions
----------------
- OPwebServer* OPwebServerCreate ( OPchar* port )
- void OPwebServerUpdate ( OPwebServer* server )
- void OPwebServerOnKey ( OPwebServer* server, OPchar* key, void() handler, void* param )
- void OPwebServerQueue ( OPwebServer* server, OPchar* key, i8* data, ui32 datalen )
- void OPwebServerDestroy ( OPwebServer* server )
- void OPwebServerQueue ( OPwebServer* server, OPchar* key, OPchar* str )
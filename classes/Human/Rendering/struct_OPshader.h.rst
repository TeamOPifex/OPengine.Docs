OPshader.h
=========

OPshaderAttribute
----------------
- OPchar* Name
- ui32 Type
- ui32 Elements
- OPuint Offset
- OPuint Handle
Globals
----------------
Functions
----------------
- OPint OPshaderLoadVertex ( OPstream* str, OPshader* shader )
- OPint OPshaderLoadFragment ( OPstream* str, OPshader* shader )
- OPint OPshaderUnload ( OPshader* shader )
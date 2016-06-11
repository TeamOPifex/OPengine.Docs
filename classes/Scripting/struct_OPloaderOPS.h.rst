OPloaderOPS.h
=========

OPscript
----------------
- OPchar* data
- i8 changed
Globals
----------------
Functions
----------------
- OPint OPscriptLoad ( const OPchar* filename, OPscript* script )
- OPint OPscriptUnload ( OPscript* script )
- OPint OPscriptReload ( const OPchar* filename, OPscript* script )
- void OPscriptAddLoader (  )
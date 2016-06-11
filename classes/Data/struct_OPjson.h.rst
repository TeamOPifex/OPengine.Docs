OPjson.h
=========

OPjson
----------------
- json_t* _json
Globals
----------------
Functions
----------------
- OPjson OPjsonLoad ( const OPchar* data )
- ui32 OPjsonElements ( OPjson json )
- ui32 OPjsonArraySize ( OPjson json )
- OPjson OPjsonGet ( OPjson json, const OPchar* key )
- OPjson OPjsonArrayGet ( OPjson json, ui32 index )
- const OPchar* OPjsonString ( OPjson json )
- i64 OPjsonI64 ( OPjson json )
- f32 OPjsonF32 ( OPjson json )
- i8 OPjsonBool ( OPjson json )
-  OPjsonType ( OPjson json )
- void OPjsonLog ( OPjson root )
- void OPjsonDestroy ( OPjson json )
- OPint OPjsonCmanLoad ( OPstream* str, void* asset )
- OPint OPjsonCmanUnload ( void* asset )
- const OPchar* OPjsonString ( OPjson json, const OPchar* key )
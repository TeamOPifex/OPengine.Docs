LoaderOPLVL.h
=========

OPLevelEntity
----------------
- OPchar* name
- OPchar* resource
- OPvec3 position
- OPvec3 rotation
- OPvec3 scale
- ui16 collision
- ui16 physics
OPLevel
----------------
- ui16 count
- OPLevelEntity* entities
Globals
----------------
Functions
----------------
- OPLevelEntity* OPlevelGetEntity ( OPLevel* level, OPchar* name )
- OPint OPlevelload ( const OPchar* filename, OPLevel* level )
- OPint OPlevelReload ( const OPchar* filename, OPLevel* level )
- OPint OPlevelUnload ( void* image )
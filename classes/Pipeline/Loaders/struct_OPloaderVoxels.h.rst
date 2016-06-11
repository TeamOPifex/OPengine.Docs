OPloaderVoxels.h
=========

OPvecInt3
----------------
- OPint x
- OPint y
- OPint z
OPvoxels
----------------
- OPvecInt3 size
- OPvecInt3 offset
- OPvecInt3* voxels
Globals
----------------
Functions
----------------
- OPint OPvoxelsLoad ( OPstream* path, void* asset )
- OPvecInt3 OPvoxelsGet ( OPvoxels* voxels, OPint x, OPint y, OPint z )
- OPassetLoader* OPvoxelsLoader (  )
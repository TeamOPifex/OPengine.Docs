OPsphericalCube.h
=========

OPsphericalCubeVertex
----------------
- OPvec3 pos
- OPvec3 norm
- OPvec2 uv
OPsphericalCube
----------------
-  sides
Globals
----------------
Functions
----------------
- OPsphericalCube OPsphericalCubeCreate ( OPimage* faces )
- OPsphericalCube OPsphericalCubeCreate ( ui16 size )
- OPvec3 OPsphericalCubePosition ( OPvec3 pos,  side )
- OPvec2 OPsphericalCubePlanePositionSide ( const OPvec3 pos,  side )
- OPvec2 OPsphericalCubePlanePosition ( const OPvec3 pos,  side )
- void OPsphericalCubeDestroy ( OPsphericalCube* sphericalCube )
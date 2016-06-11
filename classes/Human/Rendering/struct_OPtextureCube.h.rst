OPtextureCube.h
=========

OPtextureCube
----------------
- ui16 Width
- ui16 Height
- OPtexture Texture
Globals
----------------
Functions
----------------
- void OPtextureCubeInit ( OPtextureCube* result, OPimage* faces )
- OPtextureCube* OPtextureCubeCreate ( OPimage* faces )
- void OPtextureCubeDestroy ( OPtextureCube* result )
- void OPtextureCubeFree ( OPtextureCube* result )
- void OPtextureCubeClearActive (  )
- ui32 OPtextureCubeBind ( OPtextureCube* result )
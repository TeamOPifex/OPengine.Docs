OPimagePNG.h
=========

Globals
----------------
Functions
----------------
- void OPimagePNG24WriteStream ( ui8* imageData, i32 width, i32 height, ui8* data, OPuint* dataSize )
- void OPimagePNG32WriteStream ( ui8* imageData, i32 width, i32 height, ui8* data, OPuint* dataSize )
- void OPimagePNGCreate24 ( ui8* imageData, i32 width, i32 height, OPchar* filename )
- void OPimagePNGCreate32 ( ui8* imageData, i32 width, i32 height, OPchar* filename )
- i32 OPimagePNGLoad ( OPstream* str, OPtexture* image )
- i32 OPimagePNGLoadStream ( OPstream* str, OPuint offset, OPtexture* image )
- OPimage OPimagePNGLoadData ( const OPchar* filename )
- i32 OPimagePNGReload ( OPstream* str, OPtexture* image )
- i32 OPimagePNGUnload ( void* image )
OPfontAtlas.h
=========

OPfontAtlasNode
----------------
- i32 x
- i32 y
- i32 z
OPfontAtlasRegion
----------------
- i32 x
- i32 y
- i32 width
- i32 height
OPfontAtlas
----------------
- OPvector* nodes
- i32 width
- i32 height
- OPint depth
- OPint used
- ui8* data
Globals
----------------
Functions
----------------
- OPfontAtlas* OPfontAtlasCreate ( i32 width, i32 height, OPint depth )
- void OPfontAtlasDestroy ( OPfontAtlas* atlas )
- void OPfontAtlasSetRegion ( OPfontAtlas* atlas, OPint x, OPint y, OPint width, OPint height, ui8* data, OPint stride )
- OPint OPfontAtlasFit ( OPfontAtlas* atlas, OPint index, OPint width, OPint height )
- void OPfontAtlasMerge ( OPfontAtlas* atlas )
- OPfontAtlasRegion OPfontAtlasGetRegion ( OPfontAtlas* atlas, i32 width, i32 height )
- OPtexture OPfontAtlasTexture ( OPfontAtlas* atlas )
- void OPfontAtlasSavePNG ( OPfontAtlas* atlas, OPchar* filename )
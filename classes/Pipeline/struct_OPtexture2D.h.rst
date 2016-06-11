OPtexture2D.h
=========

OPtexture2D
----------------
- OPvec2 Position
- OPfloat Rotation
- OPvec2 Scale
- OPtexture* Texture
- OPeffect* Effect
Globals
----------------
Functions
----------------
- OPtexture2D* OPtexture2DCreate ( OPtexture* texture, OPeffect* effect, OPvec2 uvStart, OPvec2 uvEnd )
- OPtexture2D* OPtexture2DCreate ( OPtexture* texture, OPeffect* effect )
- void OPtexture2DDestroy ( OPtexture2D* character )
- void OPtexture2DPrepRender ( OPtexture2D* tex2d )
- void OPtexture2DRender ( OPtexture2D* tex2d )
- void OPtexture2DUnloadGlobals (  )
- OPtexture2D* OPtexture2DCreate ( OPtexture* texture )
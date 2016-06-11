OPtexture.h
=========

OPtextureDescription
----------------
- ui16 Width
- ui16 Height
- ui32 InternalFormat
- ui32 Format
- ui32 DataType
- ui32 MinFilter
- ui32 MagFilter
- ui32 WrapX
- ui32 WrapY
- ui32 CompareFunc
- ui32 CompareMode
OPtexture
----------------
- OPtextureDescription Description
- ui32 Handle
Globals
----------------
- OPtexture* OPRENDER_CURR_TEX
Functions
----------------
- OPtexture OPtextureCreate ( OPtextureDescription desc )
- void OPtextureDestroy ( OPtexture* tex )
- ui32 OPtextureBind ( OPtexture* tex )
- void OPtextureClearActive (  )
- void OPtextureSetData ( void* data )
- void OPtexturePixelate (  )
- void OPtextureSmooth (  )
- OPvec4 OPtextureReadPixel ( OPtexture* tex, OPint x, OPint y )
- OPtexture* OPtextureLoad ( const OPchar* asset )
OPeffect.h
=========

OPeffect
----------------
- OPshader Vertex
- OPshader Fragment
- ui32 ProgramHandle
- ui32 Stride
- OPhashMap* Parameters
- OPlist* Attributes
-  Name
Globals
----------------
- OPeffect* OPEFFECT_ACTIVE
Functions
----------------
- OPeffect OPeffectCreate ( OPshader vert, OPshader frag, OPshaderAttribute* Attributes, OPint AttribCount, const OPchar* Name, ui32 stride )
- OPeffect OPeffectCreate ( OPshader vert, OPshader frag, OPshaderAttribute* Attributes, OPint AttribCount, const OPchar* Name )
- OPeffect OPeffectGen ( const OPchar* vert, const OPchar* frag, ui32 attrs, const OPchar* Name, ui32 stride )
- OPeffect OPeffectGen ( const OPchar* vert, const OPchar* frag, OPvertexLayout* layout )
- OPint OPeffectUnload ( OPeffect* effect )
- void OPeffectUse ( OPeffect* effect )
- OPint OPeffectBind ( OPeffect* effect, ui32 stride )
- void* __builtin_memcpy ( void* undefined, const void* undefined, unsigned int undefined )
- OPint OPeffectBind ( OPeffect* effect )
- ui32 OPeffectGetParam ( const OPchar* parameterName )
- OPuint OPeffectParam ( const OPchar* param )
- void OPeffectParamf ( const OPchar* param, OPfloat f )
- void OPeffectParamf ( OPint loc, OPfloat f )
- void OPeffectParamfv ( const OPchar* param, OPint count, OPfloat* f )
- void OPeffectParamVec2 ( const OPchar* param, OPvec2* f )
- void OPeffectParamVec3 ( const OPchar* param, OPvec3* f )
- void OPeffectParamVec4 ( const OPchar* param, OPvec4* f )
- void OPeffectParamVec2v ( const OPchar* param, OPint count, OPvec2* f )
- void OPeffectParamVec3v ( const OPchar* param, OPint count, OPvec3* f )
- void OPeffectParamVec4v ( const OPchar* param, OPint count, OPvec4* f )
- void OPeffectParami ( const OPchar* param, OPint i )
- void OPeffectParamBindTex ( const OPchar* param, OPtexture* tex )
- void OPeffectParamBindTex ( i32 loc, OPtexture* tex )
- void OPeffectParamBindCubeMap ( const OPchar* param, OPtextureCube* tex )
- void OPeffectParamBindCubeMap ( i32 loc, OPtextureCube* tex )
- void OPeffectParamiv ( const OPchar* param, OPint count, i32* i )
- void OPeffectParamMat4 ( const OPchar* param, OPmat4* matrices )
- void OPeffectParamMat4 ( i32 loc, OPmat4* matrices )
- void OPeffectParamMat4v ( const OPchar* param, OPuint count, OPmat4* matrices )
- void OPeffectParam ( i32 loc, f32 f )
- void OPeffectParam ( const OPchar* param, f32 f )
- void OPeffectParam ( i32 loc, OPmat4 matrix )
- void OPeffectParam ( const OPchar* param, OPmat4 matrix )
- void OPeffectParam ( const OPchar* param, OPuint count, OPmat4* matrices )
- void OPeffectParam ( const OPchar* param, OPvec3 f )
- void OPeffectParam ( const OPchar* param, OPuint count, OPvec3* f )
- void OPeffectParam ( const OPchar* param, OPvec4 f )
- void OPeffectParam ( const OPchar* param, OPuint count, OPvec4* f )
- void OPeffectParam ( const OPchar* param, OPtexture* tex )
- void OPeffectParam ( const OPchar* param, OPtextureCube* tex )
- void OPeffectParam ( OPcam* camera )
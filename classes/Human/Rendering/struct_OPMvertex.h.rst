OPMvertex.h
=========

OPMmeta
----------------
- OPchar* Name
- OPchar* Type
- OPvec3 Position
- OPvec3 Rotation
- OPvec3 Scale
OPMvertex
----------------
- OPvec3 Position
- OPvec3 Normal
- OPvec3 Tangent
- OPvec2 TexCoord
OPMvertexNormalUV
----------------
- OPvec3 Position
- OPvec3 Normal
- OPvec2 UV
OPMvertexColor
----------------
- OPvec3 Position
- OPvec3 Normal
- OPvec3 Tangent
- OPvec3 Color
OPMvertexSkin
----------------
- OPvec3 Position
- OPvec3 Normal
- OPvec3 Tangent
- OPvec2 TexCoord
- OPvec4 Bones
- OPvec4 BoneWeights
OPvertexTex
----------------
- OPvec3 Position
- OPvec2 TexCoord
OPvertices
----------------
- i8* data
- ui32 features
- ui32 size
- OPuint count
Globals
----------------
Functions
----------------
- ui32 OPMhasFeature ( ui32 features,  feature )
- OPvertices* OPverticesCreate ( OPuint count, ui32 features )
- void OPverticesWriteVec2 ( OPvertices* vertices, OPvec2* data,  feature )
- void OPverticesWriteVec3 ( OPvertices* vertices, OPvec3* data,  feature )
- void OPverticesWriteVec4 ( OPvertices* vertices, OPvec4* data,  feature )
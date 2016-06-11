OPloaderOPM.h
=========

OPMdataAnim
----------------
- OPchar* Name
- OPuint FrameCount
- OPmat4* Frames
OPMData
----------------
- OPvertexLayout vertexLayout
- void* vertices
- ui32 vertexCount
- void* indices
- ui32 indexCount
- ui32 indexSize
- OPboundingBox3D bounds
- i16* hierarchy
- ui16 hierarchyCount
- OPmat4* pose
- ui16 metaCount
- OPMmeta* meta
- ui16 trackCount
- OPMdataAnim* tracks
OPMPartNode_def
----------------
- OPuint From
- OPuint To
- OPint ChildCount
- OPMPartNode* Children
Globals
----------------
Functions
----------------
- void OPMgenerateTangent ( OPvec3* tangent, OPMvertex* v1, OPMvertex* v2 )
- OPMData OPMloadData ( OPstream* str )
- OPint OPMPartitionedLoad ( const OPchar* filename, OPmesh* mesh )
- OPMData OPMloadData ( const OPchar* filename )
- OPint OPMload ( OPstream* str, OPmesh* mesh )
- OPint OPMloadPacked ( const OPchar* filename, OPmeshPacked* mesh )
- OPint OPMReload ( OPstream* str, OPmesh* mesh )
- OPint OPMUnload ( void* image )
OPvoxelGenerator.h
=========

OPvoxelGenerator
----------------
- OPuint Features
- OPuint VertexSize
- ui32 IndexOffset
-  HideFace
- OPfloat Scale
- i8 Center
- void* Vertex
- OPlist* Vertices
- OPlist* Indices
OPvoxelGeneratorVertex
----------------
- OPvec3 Position
- OPvec3 Normal
- OPvec3 Tangent
- OPvec2 UV
- OPvec3 Color
- OPvec4 Bones
- OPvec4 Weights
OPvoxelGeneratorData
----------------
-  Vertices
-  Indices
- OPvec3 Offset
- OPvec3 Color
- OPfloat Size
Globals
----------------
Functions
----------------
- void OPvoxelGeneratorInit ( OPvoxelGenerator* gen, OPuint features )
- OPvoxelGenerator* OPvoxelGeneratorCreate ( OPuint features )
- void OPvoxelGeneratorAdd ( OPvoxelGenerator* gen, OPvoxels voxelData, OPvec4 bones, OPvec4 weights, OPvec3 offset )
- OPmeshDesc OPvoxelGeneratorBuildDesc ( OPvoxelGenerator* gen )
- OPmesh* OPvoxelGeneratorBuild ( OPvoxelGenerator* gen )
- void OPvoxelGeneratorDestroy ( OPvoxelGenerator* gen )
- void OPvoxelGeneratorAdd ( OPvoxelGenerator* gen, OPvoxels voxelData )
- void OPvoxelGeneratorAdd ( OPvoxelGenerator* gen, OPvoxels voxelData, OPvec3 offset )
- void OPvoxelGeneratorAdd ( OPvoxelGenerator* gen, OPvoxels voxelData, OPvec4 bones, OPvec4 weights )
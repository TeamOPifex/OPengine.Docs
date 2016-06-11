OPmeshBuilder.h
=========

OPmeshBuilder
----------------
- ui16 VertexSize
- OPvector* Vertices
- OPvector* Indices
Globals
----------------
Functions
----------------
- void OPmeshBuilderInit ( OPmeshBuilder* builder, ui16 vertexSize )
- OPmeshBuilder* OPmeshBuilderCreate ( ui16 vertexSize )
- void OPmeshBuilderDestroy ( OPmeshBuilder* builder )
- void OPmeshBuilderAdd ( OPmeshBuilder* builder, void* one, void* two, void* three )
- void OPmeshBuilderAdd ( OPmeshBuilder* builder, void* one, void* two, void* three, void* four )
- OPmesh OPmeshBuilderGen ( OPmeshBuilder* builder )
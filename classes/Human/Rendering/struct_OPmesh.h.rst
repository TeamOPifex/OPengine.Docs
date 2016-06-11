OPmesh.h
=========

OPmeshDataMeta
----------------
- OPchar* Name
- OPchar* Type
- OPvec3 Position
- OPvec3 Rotation
- OPvec3 Scale
OPmeshDataAnim
----------------
- OPchar* Name
- OPuint FrameCount
- OPmat4* Frames
OPmeshData
----------------
- OPvertexLayout vertexLayout
- OPboundingBox3D bounds
- ui32 vertexCount
- ui32 indexCount
- ui16 hierarchyCount
- ui16 trackCount
- ui16 metaCount
- ui32 indexSize
- void* indices
- void* vertices
- i16* hierarchy
- OPmat4* pose
- OPmeshDataMeta* meta
- OPmeshDataAnim* tracks
OPmesh
----------------
- OPrenderBuffer VertexBuffer
- OPrenderBuffer IndexBuffer
- OPvertexLayout vertexLayout
- OPmeshData* meshData
- OPboundingBox3D boundingBox
- ui32 VertexCount
- void* Vertices
- ui32 IndexSize
- ui32 IndexCount
- void* Indicies
- ui16 MetaCount
- OPMmeta* Meta
- ui64 Id

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

OPmeshDesc
----------------
- void* Vertices
- ui32 VertexSize
- ui32 VertexCount
- void* Indices
- ui32 IndexSize
- ui32 IndexCount
Globals
----------------
- OPmesh* OPMESH_ACTIVE

.. epigraph::
	.. raw:: html

		_____ _ _ _<br />/ ____| | | | | |<br />| | __| | ___ | |__ __ _| |___<br />| | |_ | |/ _ \| '_ \ / _` | / __|<br />| |__| | | (_) | |_) | (_| | \__ \<br />\_____|_|\___/|_.__/ \__,_|_|___/<br />

- void* OPMESH_ACTIVE_PTR
Functions
----------------
- OPmesh OPmeshCreate (  )

.. epigraph::
	.. raw:: html

		______ _ _<br />____| | | (_)<br />|__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />__| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | |_| | | | | (__| |_| | (_) | | | \__ \<br />\__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- OPmesh* OPmeshCreate ( OPmeshDesc desc )
- void OPmeshDestroy ( OPmesh* mesh )
- void OPmeshBuild ( ui32 vertSize, ui32 indSize, OPuint vertCount, OPuint indCount, void* vertices, void* indices )
- void OPmeshRender (  )
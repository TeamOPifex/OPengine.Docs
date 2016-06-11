OPcommandDrawIndexed.h
=========

OPcommandDrawIndexed
----------------
- ui64 key
- void() dispatch
- ui32 indexCount
- ui32 startIndex
- ui32 baseVertex
- ui32 stride
- OPvertexLayout* vertexLayout
- OPrenderBuffer* vertexBuffer
- OPrenderBuffer* indexBuffer
- OPmaterial* material
- OPmat4* world
- OPtexture* texture

.. epigraph::
	.. raw:: html

		Draws a mesh that has both a vertex buffer and an index buffer<br />

Globals
----------------
Functions
----------------
- void OPcommandDrawIndexedSet ( OPcommandDrawIndexed* result, OPmodel* model, OPmaterial* material )
- void OPcommandDrawIndexedSet ( OPcommandDrawIndexed* result, OPmodel* model, OPmaterial* material, OPtexture* texture )
- void OPcommandDrawIndexedSubmit ( OPcommandBucket* commandBucket, OPmodel* model, OPmaterial* material, OPtexture* texture )
- void OPcommandDrawIndexedSubmit ( OPcommandBucket* commandBucket, OPmodelTextured* model, OPmaterial* material )
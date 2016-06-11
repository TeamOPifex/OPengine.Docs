OPcommandBucket.h
=========

OPcommandDrawCommand
----------------
- void* next
- void* data
- void() dispatch
OPcommandBucketKey
----------------
- ui64 key
- OPcommandDrawCommand* command

.. epigraph::
	.. raw:: html

		A key for the OPcommandBucket that will be sorted for rendering order<br />

OPcommandBucket
----------------
- OPuint bucketSize
- OPallocator* allocator
- ui32 keyIndex
- OPcommandBucketKey* keys
- OPcommandBucketKey* copykeys
- OPcommandDrawCommand* commands
- OPcam* camera
-  frameBuffer
- i8 controlOfAllocator
Globals
----------------
Functions
----------------
- void OPcommandBucketInit ( OPcommandBucket* commandBucket, OPuint bucketSize, OPcam* camera )
- void OPcommandBucketInit ( OPcommandBucket* commandBucket, OPuint bucketSize, OPcam* camera, OPallocator* allocator )
- OPcommandBucket* OPcommandBucketCreate ( OPuint bucketSize, OPcam* camera )
- OPcommandBucket* OPcommandBucketCreate ( OPuint bucketSize, OPcam* camera, OPallocator* allocator )
- void OPcommandBucketFlush ( OPcommandBucket* commandBucket )
- void OPcommandBucketSortKeys ( OPcommandBucket* commandBucket )
- void OPcommandBucketSubmit ( OPcommandBucket* commandBucket, ui64 key, void() dispatch, void* data, void* next )
- void OPcommandBucketSubmit ( OPcommandBucket* commandBucket, ui64 key, void() dispatch, void* data )
- void OPcommandBucketRender ( OPcommandBucket* commandBucket )
- OPcommandDrawIndexed* OPcommandBucketCreateDrawIndexed ( OPcommandBucket* commandBucket )

.. epigraph::
	.. raw:: html

		Helper draw commands already in the engine<br />Users will be able to define their own, just won't be a helper function<br />in the struct itself unless they modify the OPengine source itself<br />

OPallocLinear.h
=========

OPallocatorLinear
----------------
- OPuint _allocCount
- OPuint _usedMemory
- OPuint _size
- void* _headerStart
- void* _memStart
- void* _currentPos

.. epigraph::
	.. raw:: html

		Struct definitions */<br />Linear Memory Block<br />

Globals
----------------
Functions
----------------
- void OPallocatorLinearInit ( OPallocator* result, OPuint sizeInBytes )
- OPallocator* OPallocatorLinearCreate ( OPuint sizeInBytes )
- void OPallocatorLinearDestroy ( OPallocator* alloc )
- void* OPallocatorLinearAlloc ( OPallocator* alloc, OPuint sizeInBytes )
- void OPallocatorLinearFree ( OPallocator* alloc, void* data )
- void OPallocatorLinearReset ( OPallocator* alloc )
- OPuint OPallocatorLinearUsed ( OPallocatorLinear* alloc )
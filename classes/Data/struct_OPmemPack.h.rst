OPmemPack.h
=========

OPmemDesc
----------------
- void() Alloc
- void() Dealloc
- OPuint() Size
- void* Data
Globals
----------------
Functions
----------------
- void* OPmemPackAlloc ( OPmemDesc* segments, OPuint segCount, OPint n )

.. epigraph::
	.. raw:: html

		Allocates a block of memory to be used in segements<br />

- void OPmemPackDealloc ( void* Data, OPmemDesc* segments, OPint segCount, OPint n )
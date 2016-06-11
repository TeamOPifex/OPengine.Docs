OPmemory.h
=========

Globals
----------------
- OPint OPallocations
- OPint OPdeallocations
- OPallocator OPDEFAULT_ALLOCATOR
Functions
----------------
- void* OPalloc ( OPuint bytes )

.. epigraph::
	.. raw:: html

		Platform independent means to dynamically allocate memory.<br />

- void* OPallocZero ( OPuint bytes )

.. epigraph::
	.. raw:: html

		Platform independent means to dynamically allocate memory and zero it out.<br />

- void* OPrealloc ( void* ptr, OPuint bytes )

.. epigraph::
	.. raw:: html

		Platform independent means to dynamically reallocate memory.<br />

- void OPfree ( void* ptr )

.. epigraph::
	.. raw:: html

		Platform independent means do deallocate dynamically<br />allocated memory. If a null pointer is passed no action<br />is taken.<br />

- void* OPsysAlloc ( OPuint bytes )
- void OPsysFree ( void* ptr )
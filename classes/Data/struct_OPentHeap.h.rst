OPentHeap.h
=========

OPentHeap
----------------
- void* Entities
- OPint* InUse
- OPint EntSize
- OPint MaxIndex
- OPuint* Size
- OPuint Capacity
- OPminHeap Free
Globals
----------------
Functions
----------------
- void OPentHeapActivate ( OPentHeap* heap, OPint* i )

.. epigraph::
	.. raw:: html

		Fills the pointer i with the index of the activated entity in the EntHeap<br />

- void* OPentHeapGet ( OPentHeap* heap, OPint i )

.. epigraph::
	.. raw:: html

		Get an indexed entity out of an EntHeap<br />

- void OPentHeapKill ( OPentHeap* heap, OPint i )

.. epigraph::
	.. raw:: html

		Kill off an entity in an EntHeap. It will be re-used when OPentHeapActivate is called.<br />

- OPuint OPentHeapBytes ( OPint entsize, OPint count )

.. epigraph::
	.. raw:: html

		Gets the size required to create an EntHeap<br />

- OPentHeap* OPentHeapCreate ( void* segPtr, OPint entSize, OPint count )

.. epigraph::
	.. raw:: html

		Creates an EntHeap<br />

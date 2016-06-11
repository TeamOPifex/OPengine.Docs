OPminHeap.h
=========

OPminHeap
----------------
- OPint* _indices
- OPuint _capacity
- OPuint _size
Globals
----------------
Functions
----------------
- OPminHeap* OPminHeapCreate ( OPuint capacity )

.. epigraph::
	.. raw:: html

		Creates an OPminHeap<br />

- OPint OPminHeapDestroy ( OPminHeap* heap )

.. epigraph::
	.. raw:: html

		Destroys an OPminHeap<br />

- OPint OPminHeapPush ( OPminHeap* heap, OPint value )

.. epigraph::
	.. raw:: html

		Puts an element into an OPminHeap<br />

- OPint OPminHeapPop ( OPminHeap* heap )

.. epigraph::
	.. raw:: html

		Pops an element off the top of an OPminHeap<br />

- OPint OPminHeapPeek ( OPminHeap* heap )

.. epigraph::
	.. raw:: html

		Looks at the top element of an OPminHeap without popping it off<br />

- OPint OPminHeapSize ( OPminHeap* heap )

.. epigraph::
	.. raw:: html

		Size of the OPminHeap<br />

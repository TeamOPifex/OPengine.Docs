OPlinkedList.h
=========

OPllNode_def
----------------
- OPllNode* Prev
- OPllNode* Next
- void* Data
OPlinkedList
----------------
- OPint _size
- OPllNode* First
- OPllNode* Last
Globals
----------------
Functions
----------------
- OPlinkedList* OPllCreate (  )

.. epigraph::
	.. raw:: html

		Creates an OPlinkedList<br />

- OPint OPllDestroy ( OPlinkedList* list )

.. epigraph::
	.. raw:: html

		Destroys an OPlinkedList<br />

- OPllNode* OPllInsertFirst ( OPlinkedList* list, void* data )

.. epigraph::
	.. raw:: html

		Inserts a node into the first position of an OPlinkedList<br />

- OPllNode* OPllInsertLast ( OPlinkedList* list, void* data )

.. epigraph::
	.. raw:: html

		Inserts a node into the last position of an OPlinkedList<br />

- void* OPllRemove ( OPlinkedList* list, OPllNode* toRemove )

.. epigraph::
	.. raw:: html

		Removes an OPllNode from an OPlinkedList<br />

- OPint OPllGetSize ( OPlinkedList* list )

.. epigraph::
	.. raw:: html

		Gets the number of elements stored in the OPlinkedList<br />

OPlist.h
=========

OPlist
----------------
- ui8* _indices
- OPuint _capacity
- OPuint _size
- OPuint _elementSize

.. epigraph::
	.. raw:: html

		An OPlist<br />

Globals
----------------
Functions
----------------
- OPlist* OPlistCreate ( OPint capacity, OPint elementSize )

.. epigraph::
	.. raw:: html

		Creates a new OPlist<br />

- OPint OPlistDestroy ( OPlist* list )

.. epigraph::
	.. raw:: html

		Destroys an OPlist<br />

- OPint OPlistPush ( OPlist* list, ui8* value )

.. epigraph::
	.. raw:: html

		Copies an element into the OPlist<br />The value is mem copied into the list so the value passed can be safely freed<br />

- ui8* OPlistPop ( OPlist* list )

.. epigraph::
	.. raw:: html

		Pops the last element of the OPlist<br />

- ui8* OPlistPeek ( OPlist* list )

.. epigraph::
	.. raw:: html

		Peeks at the last element of the OPlist<br />

- OPint OPlistInsert ( OPlist* list, ui8* value, OPuint index )

.. epigraph::
	.. raw:: html

		Inserts an element at an index to an OPlist<br />

- OPint OPlistRemoveAt ( OPlist* list, OPuint index )

.. epigraph::
	.. raw:: html

		Removes an element at an index of an OPlist<br />

- ui8* OPlistGet ( OPlist* list, OPuint index )

.. epigraph::
	.. raw:: html

		Gets an element at an index of an OPlist<br />

- ui8* OPlistSet ( OPlist* list, OPuint index, ui8* value )

.. epigraph::
	.. raw:: html

		Sets an element at an index of an OPlist<br />This will overwrite anything at the specified index<br />

- OPuint OPlistSize ( OPlist* list )

.. epigraph::
	.. raw:: html

		Current size of an OPlist<br />

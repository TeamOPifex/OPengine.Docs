OPhashMap.h
=========

KeyValuePair
----------------
- OPchar* key
- void* value

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />(___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />\__|_| \__,_|\___|\__|___/<br />

Bucket
----------------
- OPuint count
- KeyValuePair* pairs
OPhashMap
----------------
- OPuint count
- Bucket* buckets
Globals
----------------
Functions
----------------
- void OPhashMapInit ( OPhashMap* hashMap, OPuint capacity )
- OPhashMap* OPhashMapCreate ( OPuint capacity )

.. epigraph::
	.. raw:: html

		Creates a HashMap (Dictionary)<br />

- void OPhashMapDestroy ( OPhashMap* map )

.. epigraph::
	.. raw:: html

		Destroys an OPhashMap<br />

- OPint OPhashMapGet ( const OPhashMap* hashMap, const OPchar* key, void* value )

.. epigraph::
	.. raw:: html

		Gets a value out of an OPhashMap<br />

- OPint OPhashMapExists ( const OPhashMap* map, const OPchar* key )

.. epigraph::
	.. raw:: html

		Determines if an OPhashMap contains a value with a key<br />

- OPint OPhashMapPut ( OPhashMap* map, const OPchar* key, void* value )

.. epigraph::
	.. raw:: html

		Puts a value by a key into an OPhashMap. If all buckets have been used it will fail.<br />

- OPint OPhashMapCount ( const OPhashMap* map )

.. epigraph::
	.. raw:: html

		Gets the number of buckets being used by an OPhashMap<br />

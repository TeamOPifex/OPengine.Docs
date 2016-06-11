OPstream.h
=========

OPstream
----------------
- OPuint Length
- OPuint Size
-  Buffer
- OPuint _pointer
- OPchar* Source
- ui8* Data
Globals
----------------
Functions
----------------
- OPstream* OPstreamCreate ( OPuint size )

.. epigraph::
	.. raw:: html

		OPstreamCreate - Allocates a byte stream instance.<br />

- OPuint OPstreamDestroy ( OPstream* stream )

.. epigraph::
	.. raw:: html

		OPstreanDestroy - Deallocates memory used by a stream.<br />

- OPuint OPwrite ( OPstream* stream, void* data, OPuint size )

.. epigraph::
	.. raw:: html

		OPwrite - Append data to the stream.<br />

- ui8* OPread ( OPstream* stream, OPuint size )

.. epigraph::
	.. raw:: html

		OPread - Reads data and advances the pointer.<br />no allocation performed.<br />

- i8 OPstreamI8 ( OPstream* stream )
- i16 OPstreamI16 ( OPstream* stream )
- i32 OPstreamI32 ( OPstream* stream )
- ui8 OPstreamUI8 ( OPstream* stream )
- ui16 OPstreamUI16 ( OPstream* stream )
- ui32 OPstreamUI32 ( OPstream* stream )
- f32 OPstreamf32 ( OPstream* stream )
- OPchar* OPstreamString ( OPstream* stream )

.. epigraph::
	.. raw:: html

		Reads the first string it finds in the stream<br />Defined by a separated space.<br />Ex: 'Apple Banana Pear' would return Apple<br />

- OPchar* OPstreamReadLine ( OPstream* stream )

.. epigraph::
	.. raw:: html

		Reads the next line available in the OPstream<br />Reads until it finds a \n and will remove all \r<br />

- OPint OPstreamReadKeyValuePair ( OPstream* stream, OPkeyValuePair* dst )

.. epigraph::
	.. raw:: html

		Reads a text key value pair<br />Ex: ' Test = My Value ' would return a KeyValue of<br />Key : Test<br />Value : My Value<br />

- ui8* OPreadAt ( OPstream* stream, OPuint pos, OPuint size )

.. epigraph::
	.. raw:: html

		OPreadAt - Reads data at a specific location.<br />no allocation performed.<br />

- OPuint OPcopy ( OPstream* stream, void* dest, OPuint size )

.. epigraph::
	.. raw:: html

		OPcopy - Reads data, and copies it into a provided buffer<br />

- OPuint OPseek ( OPstream* stream, OPuint byte )

.. epigraph::
	.. raw:: html

		OPseek - Skip to a specific byte location in the stream.<br />

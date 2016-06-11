OPfile.h
=========

OPfile
----------------
- FILE* _handle
- const OPchar* path
OPfileInformation
----------------
- FILE* file
- ui32 start
- ui32 length
- int fileDescriptor
Globals
----------------
Functions
----------------
- ui16 OPreadui16 ( OPstream* str )

.. epigraph::
	.. raw:: html

		OPreadui16 - Reads the next 2 bytes from the file and converts to ui16<br />

- ui32 OPreadui32 ( OPstream* str )

.. epigraph::
	.. raw:: html

		OPreadui32 - Reads the next 4 bytes from the file and converts to ui32<br />

- OPchar OPreadi8 ( OPstream* str )

.. epigraph::
	.. raw:: html

		OPreadi8 - Reads the next 1 byte from the file and converts to i8<br />

- i16 OPreadi16 ( OPstream* str )

.. epigraph::
	.. raw:: html

		OPreadi16 - Reads the next 2 bytes from the file and converts to i16<br />

- i32 OPreadi32 ( OPstream* str )

.. epigraph::
	.. raw:: html

		OPreadi32 - Reads the next 4 bytes from the file and converts to i32<br />

- f32 OPreadf32 ( OPstream* str )

.. epigraph::
	.. raw:: html

		OPreadf32 - Reads the next 4 bytes from the file and converts to f32<br />

- OPchar* OPreadstring ( OPstream* str )

.. epigraph::
	.. raw:: html

		OPreadstring - Reads the next string from the file<br />

- OPfileInformation OPreadFileInformation ( const char* path )

.. epigraph::
	.. raw:: html

		OPreadFileInformation - Reads file information, getting start and length<br />

- OPint OPwriteFile ( const char* path, OPstream* data )

.. epigraph::
	.. raw:: html

		OPwriteFile - Writes a byte stream to a file.<br />

- OPstream* OPreadFile ( const char* path )

.. epigraph::
	.. raw:: html

		OPreadFile - Reads a file into a byte stream.<br />

- OPstream* OPreadFileLarge ( const char* path, ui32 expectedSize )

.. epigraph::
	.. raw:: html

		OPreadFile - Reads a file into a byte stream.<br />

- OPint OPfileExists ( const char* path )

.. epigraph::
	.. raw:: html

		OPfileExists - Checks for the existance of a file.<br />

- OPint OPdeleteFile ( const char* path )

.. epigraph::
	.. raw:: html

		OPdeleteFile - Deletes a file from the filesystem.<br />

- ui64 OPfileLastChange ( const OPchar* path )
- OPfile OPfileOpen ( const OPchar* path )
- OPstream* OPfileRead ( OPfile* path, ui32 size )
- OPint OPfileWriteui8 ( OPfile* file, ui8 data )
- OPint OPfileWriteui16 ( OPfile* file, ui16 data )
- OPint OPfileWriteui32 ( OPfile* file, ui32 data )
- OPint OPfileWritei8 ( OPfile* file, i8 data )
- OPint OPfileWritei16 ( OPfile* file, i16 data )
- OPint OPfileWritei32 ( OPfile* file, i32 data )
- OPint OPfileWriteString ( OPfile* file, const OPchar* data )
- OPint OPfileWriteBytes ( OPfile* file, void* data, ui64 bytesToWrite )
- ui8 OPfileReadui8 ( OPfile* file )
- ui16 OPfileReadui16 ( OPfile* file )
- ui32 OPfileReadui32 ( OPfile* file )
- i8 OPfileReadi8 ( OPfile* file )
- i16 OPfileReadi16 ( OPfile* file )
- i32 OPfileReadi32 ( OPfile* file )
- OPchar* OPfileReadString ( OPfile* file )
- void* OPfileReadBytes ( OPfile* file, ui64 bytesToRead )
- OPint OPfileSeekReset ( OPfile* file )
- OPint OPfileSeek ( OPfile* file, OPint pos )
- OPint OPfileClose ( OPfile* file )
- OPfileInformation OPfileCreate ( const char* path )
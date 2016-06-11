OPlog.h
=========

Globals
----------------
- i32 LogToHandle
- ui32 OP_LOG_LEVEL
- void() OPlogHandler
Functions
----------------
- void OPlogSetOutput ( i32 handle )
- void OPlg ( const char* message )

.. epigraph::
	.. raw:: html

		Prints out to the console, accepts variable arguments like sprintf<br />

- void OPlog ( const char* message )

.. epigraph::
	.. raw:: html

		Prints out to the console, accepts variable arguments like sprintf,<br />does not write a new line at the end of the message<br />

- void OPvlog ( ui32 level, const char* channel, const char* message, va_list args )
- void OPlogChannel ( i32 level, const char* channel, const char* message )
- void OPlogDebug ( const char* message )

.. epigraph::
	.. raw:: html

		Level 10<br />

- void OPlogInfo ( const char* message )

.. epigraph::
	.. raw:: html

		Level 30<br />

- void OPlogWarn ( const char* message )

.. epigraph::
	.. raw:: html

		Level 20<br />

- void OPlogErr ( const char* message )

.. epigraph::
	.. raw:: html

		Level 0<br />

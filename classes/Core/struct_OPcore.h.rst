OPcore.h
=========

Globals
----------------
Functions
----------------
- void OPstart ( int argc, char* args )

.. epigraph::
	.. raw:: html

		Begins the game cycle.<br />This function is responsible for several actions. It creates an<br />OPtimer instance, and invokes the function pointer OPinitialize() to<br />perform user defined initializations. Once initialized, the game loop<br />is started. The timer instance is updated on each iteration and passed<br />to the OPupdate function pointer. The game loop runs until OPend() is<br />called. At which point the OPdestroy() function pointer is called and<br />and clean up is performed.<br />

- void OPstartStepped ( int argc, char* args )
- void OPend (  )

.. epigraph::
	.. raw:: html

		Ends the game cycle.<br />This function sets an internal flag which will cease the game loop.<br />and result in the termination and clean up of all user code and<br />data.<br />

- OPtimer* OPgetTime (  )

.. epigraph::
	.. raw:: html

		Gets the current OPtimer being used by the engine<br />

- OPchar* OPgetStartupDir (  )
- OPchar* OPgetExecutableDir (  )
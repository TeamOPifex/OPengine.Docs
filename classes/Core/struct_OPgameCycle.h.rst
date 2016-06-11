OPgameCycle.h
=========

Globals
----------------
- void() OPinitialize

.. epigraph::
	.. raw:: html

		Game engine initialization.<br />This function pointer points to a user function which is responsible<br />for performing any essential initialization, data allocation and setup<br />which is needed to begin the primary game loop.<br />

- OPint() OPupdate

.. epigraph::
	.. raw:: html

		Game engine update.<br />This function pointer points to a user function which accepts an<br />OPtimer as an argument. This function performs whatever action needs<br />to be taken to actually run the game. For example, this function would<br />be responsible for invoking game-logic updates, input device polling<br />and scene rendering.<br />

- void() OPrender

.. epigraph::
	.. raw:: html

		Game engine render.<br />This function pointer points to a user function which accepts an<br />OPfloat as an argument. This function performs whatever actions are<br />needed to do scene rendering.<br />

- void() OPdestroy

.. epigraph::
	.. raw:: html

		Game engine termination.<br />This function pointer points to a user function which is responsible<br />for gracefully terminating the game engine. This may include saving<br />data, deallocating memory, releasing OS resources and closing<br />network connections.<br />

Functions
----------------
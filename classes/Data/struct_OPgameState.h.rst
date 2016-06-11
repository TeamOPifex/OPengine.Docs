OPgameState.h
=========

OPgameState
----------------
- void() Init
- OPint() Update
- void() Render
- OPint() Exit
- void* Data
Globals
----------------
- OPgameState* ActiveState
Functions
----------------
- void OPgameStateChange ( OPgameState* targetState )

.. epigraph::
	.. raw:: html

		Changes the current game state, on change calls the Exit on the current game state, and then the initialize on the new game state<br />

- OPgameState* OPgameStateCreate ( void() init, OPint() update, OPint() exit )

.. epigraph::
	.. raw:: html

		Creates a new OPgameState<br />

- OPint OPgameStateDestroy ( OPgameState* state )

.. epigraph::
	.. raw:: html

		Destroys an OPgameState by deallocating the memory<br />

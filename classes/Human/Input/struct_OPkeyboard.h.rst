OPkeyboard.h
=========

OPkeyboardState
----------------
-  keys
-  prevKeys
Globals
----------------
- OPkeyboardState Keyboard
- void() OPKEYBOARD_STREAM
Functions
----------------
- void OPkeyboardUpdate ( OPtimer* timer )
- void OPkeyboardUpdatePost ( OPtimer* timer )
- OPint OPkeyboardIsDown (  key )
- OPint OPkeyboardIsUp (  key )
- OPint OPkeyboardWasPressed (  key )
- OPint OPkeyboardWasReleased (  key )
- OPint OPkeyboardAnyInputIsDown (  )
- void OPkeyboardKey ( OPuint codepoint )
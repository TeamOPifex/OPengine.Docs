OPmouse.h
=========

OPmouseState
----------------
- i32 updatedWheel
- i32 wheel
- i32 prevWheel
- d64 positionX
- d64 positionY
- d64 prevPositionX
- d64 prevPositionY
-  keys
-  prevKeys
Globals
----------------
- OPmouseState Mouse
Functions
----------------
- void OPmouseUpdate (  )
- i32 OPmousePositionX (  )
- i32 OPmousePositionY (  )
- i32 OPmousePositionMovedX (  )
- i32 OPmousePositionMovedY (  )
- i32 OPmouseWheel (  )
- i32 OPmouseWheelMoved (  )
- OPint OPmouseIsDown (  key )
- OPint OPmouseIsUp (  key )
- OPint OPmouseWasPressed (  key )
- OPint OPmouseWasReleased (  key )
- void OPmouseSetPosition ( i32 x, i32 y )
- void OPmouseSetPositionScreenCenter (  )
- OPint OPmouseAnyInputIsDown (  )
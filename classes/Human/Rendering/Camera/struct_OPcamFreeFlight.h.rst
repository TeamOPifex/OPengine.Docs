OPcamFreeFlight.h
=========

OPcamFreeFlight
----------------
- OPcam Camera
- OPvec3 Rotation
- OPvec3 Movement
- OPfloat RotationSpeed
- OPfloat MoveSpeed

.. epigraph::
	.. raw:: html

		Free Flight Camera<br />

Globals
----------------
Functions
----------------
- void OPcamFreeFlightInit ( OPcamFreeFlight* camFree, OPfloat moveSpeed, OPfloat rotateSpeed, OPvec3 position, OPfloat camNear, OPfloat camFar )
- OPcamFreeFlight* OPcamFreeCreate ( OPfloat moveSpeed, OPfloat rotateSpeed, OPvec3 position, OPfloat camNear, OPfloat camFar )
- void OPcamFreeFlightUpdate ( OPcamFreeFlight* camFree, OPtimer* timer )
- void OPcamFreeFlightUpdate ( OPcamFreeFlight* camFree )
- void OPcamFreeFlightDestroy (  )
- void OPcamFreeFlightInit ( OPcamFreeFlight* camFree, OPfloat moveSpeed, OPfloat rotateSpeed, OPvec3 position )
- OPcamFreeFlight* OPcamFreeCreate ( OPfloat moveSpeed, OPfloat rotateSpeed, OPvec3 position )
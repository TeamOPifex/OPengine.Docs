OPvec3.h
=========

OPvec3
----------------
-  
OPmat4
----------------

----------------
- OPfloat x
- OPfloat y
- OPfloat z
Globals
----------------
- const OPvec3 OPVEC3_ZERO
- const OPvec3 OPVEC3_ONE
- const OPvec3 OPVEC3_UP
- const OPvec3 OPVEC3_LEFT
- const OPvec3 OPVEC3_FORWARD
- const OPvec3 OPVEC3_BACKWARD
Functions
----------------
- OPvec3 OPvec3Create ( OPfloat x, OPfloat y, OPfloat z )
- void OPvec3Add ( OPvec3* dst, OPvec3* a, OPvec3* b )
- void OPvec3Sub ( OPvec3* dst, OPvec3* a, OPvec3* b )
- void OPvec3Mul ( OPvec3* dst, OPvec3* a, OPvec3* b )
- void OPvec3Scl ( OPvec3* dst, OPvec3* a, OPfloat s )
- void OPvec3Div ( OPvec3* dst, OPvec3* a, OPvec3* b )
- void OPvec3Div ( OPvec3* dst, OPvec3* a, OPfloat b )
- OPfloat OPvec3AngleToTarget ( OPvec3 pos, OPvec3 facing, OPvec3 target )
- OPvec3 OPvec3Create ( OPvec2 xy, OPfloat z )
- OPvec3 OPvec3Create ( OPfloat x )
- OPfloat OPvec3Dot ( OPvec3 a, OPvec3 b )

.. epigraph::
	.. raw:: html

		___ _ _ _ _ _ _ _ _ _<br />| __| _ _ _ __| |_(_)___ _ _ __ _| | /_\ _ _(_) |_| |_ _ __ ___| |_(_)__<br />| _| || | ' \/ _| _| / _ \ ' \/ _` | | / _ \| '_| | _| ' \| ' \/ -_) _| / _|<br />|_| \_,_|_||_\__|\__|_\___/_||_\__,_|_| /_/ \_\_| |_|\__|_||_|_|_|_\___|\__|_\__|<br />

- OPvec3 OPvec3Cross ( OPvec3 a, OPvec3 b )
- OPfloat OPvec3Len ( OPvec3 v )
- OPfloat OPvec3Dist ( OPvec3 a, OPvec3 b )
- OPfloat OPvec3DistSquare ( OPvec3 a, OPvec3 b )
- OPfloat OPvec3Angle ( OPvec3 a, OPvec3 b )
- OPvec3 OPvec3Reflect ( OPvec3 v, OPvec3 n )
- OPvec3 OPvec3Norm ( OPvec3 v )
- OPvec3 OPvec3Abs ( OPvec3 v )
- OPvec3 OPvec3Read ( OPstream* str )
- void OPvec3Write ( OPvec3 v, OPstream* str )
- OPvec3 OPvec3RandNorm (  )
- void OPvec3Log ( const OPchar* m, OPvec3 v )
- OPvec3 OPvec3Tween ( OPvec3 a, OPvec3 b, OPfloat delta )
OPvec2.h
=========

OPvec2
----------------
-  

----------------
- OPfloat x
- OPfloat y
Globals
----------------
- const OPvec2 OPVEC2_ZERO
- const OPvec2 OPVEC2_ONE
Functions
----------------
- void OPvec2Add ( OPvec2* dst, OPvec2* a, OPvec2* b )
- void OPvec2Sub ( OPvec2* dst, OPvec2* a, OPvec2* b )
- void OPvec2Mul ( OPvec2* dst, OPvec2* a, OPvec2* b )
- void OPvec2Scl ( OPvec2* dst, OPvec2* a, OPfloat s )
- void OPvec2Div ( OPvec2* dst, OPvec2* a, OPvec2* b )
- void OPvec2Div ( OPvec2* dst, OPvec2* a, OPfloat b )
- OPfloat OPvec2Dot ( OPvec2 a, OPvec2 b )

.. epigraph::
	.. raw:: html

		___ _ _ _ _ _ _ _ _ _<br />| __| _ _ _ __| |_(_)___ _ _ __ _| | /_\ _ _(_) |_| |_ _ __ ___| |_(_)__<br />| _| || | ' \/ _| _| / _ \ ' \/ _` | | / _ \| '_| | _| ' \| ' \/ -_) _| / _|<br />|_| \_,_|_||_\__|\__|_\___/_||_\__,_|_| /_/ \_\_| |_|\__|_||_|_|_|_\___|\__|_\__|<br />

- OPfloat OPvec2Cross ( OPvec2 a, OPvec2 b )
- OPfloat OPvec2Len ( OPvec2 v )
- OPvec2 OPvec2Norm ( OPvec2 a )
- OPvec2 OPvec2Perp ( OPvec2 a )
- OPfloat OPvec2Dist ( OPvec2 a, OPvec2 b )
- OPvec2 OPvec2Reflect ( OPvec2 horizon, OPvec2 v )
- OPfloat OPvec2Angle ( OPvec2 a, OPvec2 b )
- OPvec2 OPvec2Read ( OPstream* str )
- OPvec2 OPvec2RandNorm (  )
- void OPvec2Write ( OPvec2 v, OPstream* str )
- void OPvec2Log ( const OPchar* m, OPvec2 v )
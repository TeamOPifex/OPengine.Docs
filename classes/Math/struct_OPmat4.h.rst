OPmat4.h
=========

OPmat4
----------------
-  cols

.. epigraph::
	.. raw:: html

		Data Structure 4 * 4 = 16 floats<br />32 bit = 16 * 32 = 512 bits or 64 bytes<br />64 bit = 16 * 64 = 1024 bits or 128 bytes<br />

Globals
----------------
- const OPmat4 OPMAT4_ZERO

.. epigraph::
	.. raw:: html

		EXTERNALS<br />

- const OPmat4 OPMAT4_IDENTITY
Functions
----------------
- OPmat4 OPmat4Mul ( OPmat4 m1, OPmat4 m2 )

.. epigraph::
	.. raw:: html

		INLINE PRE DECLARATIONS<br />

- void OPmat4Mul ( OPmat4* dst, OPmat4 m1, OPmat4 m2 )
- OPmat4 OPmat4RotX ( OPfloat t )
- void OPmat4RotX ( OPmat4* m, OPfloat x )
- OPmat4 OPmat4RotY ( OPfloat t )
- void OPmat4RotY ( OPmat4* m, OPfloat x )
- OPmat4 OPmat4RotZ ( OPfloat t )
- void OPmat4RotZ ( OPmat4* m, OPfloat x )
- OPmat4 OPmat4Translate ( OPfloat x, OPfloat y, OPfloat z )
- void OPmat4Translate ( OPmat4* m, OPfloat x, OPfloat y, OPfloat z )
- OPmat4 OPmat4Scl ( OPfloat x )
- OPmat4 OPmat4Scl ( OPfloat x, OPfloat y, OPfloat z )
- void OPmat4Scl ( OPmat4* m, OPfloat x, OPfloat y, OPfloat z )
- OPvec2 OPmat4Transform ( OPvec2 a, OPmat4 b )
- OPvec3 OPmat4Transform ( OPvec3 a, OPmat4 b )
- OPvec4 OPmat4Transform ( OPvec4 a, OPmat4 b )
- OPmat4 OPmat4Create ( f32 _00, f32 _10, f32 _20, f32 _30, f32 _01, f32 _11, f32 _21, f32 _31, f32 _02, f32 _12, f32 _22, f32 _32, f32 _03, f32 _13, f32 _23, f32 _33 )
- OPmat4 OPmat4Create ( OPvec4 row0, OPvec4 row1, OPvec4 row2, OPvec4 row3 )
- void OPmat4Identity ( OPmat4* m )
- OPmat4 OPmat4Transpose ( OPmat4 m )
- OPvec3 OPmat4GetTranslate ( OPmat4 mat )
- OPmat4 OPmat4Translate ( OPvec3 v )
- OPmat4 OPmat4Translate ( OPvec2 v )
- OPmat4 OPmat4RotX ( OPmat4 m, OPfloat x )
- OPmat4 OPmat4RotY ( OPmat4 m, OPfloat x )
- OPmat4 OPmat4RotZ ( OPmat4 m, OPfloat x )
- OPmat4 OPmat4Scl ( OPmat4 m, OPfloat x, OPfloat y, OPfloat z )
- OPmat4 OPmat4Scl ( OPmat4 m, OPfloat x )
- OPmat4 OPmat4Translate ( OPmat4 m, OPfloat x, OPfloat y, OPfloat z )
- OPmat4 OPmat4SetTranslate ( OPmat4 m, OPfloat x, OPfloat y, OPfloat z )
- OPmat4 OPmat4Translate ( OPmat4 m, OPvec3 v )
- OPmat4 OPmat4SetTranslate ( OPmat4 m, OPvec3 v )
- void OPmat4BuildQuat ( OPmat4* dst, OPquat* qtr )

.. epigraph::
	.. raw:: html

		NOTE(garrett): Pretty sure this unneeded now that we have OPquat<br />I think we still need it, we can use a quat to compound<br />but we may still need to retrieve them as a matrix<br />use with shaders<br />

- OPmat4 OPmat4From ( OPquat a )
- OPfloat OPmat4GetCofactor ( OPfloat m0, OPfloat m1, OPfloat m2, OPfloat m3, OPfloat m4, OPfloat m5, OPfloat m6, OPfloat m7, OPfloat m8 )
- void OPmat4Log ( const OPchar* msg, OPmat4 m )
- OPmat4 OPmat4Read ( OPstream* str )
- void OPmat4Write ( OPmat4 v, OPstream* str )
- OPmat4 OPmat4RotationBetween ( OPvec3 start, OPvec3 dest )
- OPmat4 OPmat4RotationNormal ( OPvec3 normal )
- OPmat4 OPmat4RotationNormal2 ( OPvec3 normal )
- OPmat4 OPmat4RemoveScale ( OPmat4 a )
- OPvec3 OPmat4Eulor ( OPmat4 a )
- OPmat4 OPmat4Ortho ( OPfloat left, OPfloat right, OPfloat bottom, OPfloat top, OPfloat zNear, OPfloat zFar )
- OPmat4 OPmat4LookAt ( OPvec3 eye, OPvec3 at, OPvec3 up )
- OPmat4 OPmat4Perspective ( OPfloat fovy, OPfloat aspect, OPfloat nearVal, OPfloat farVal )
- OPint OPmat4Inverse ( OPmat4* dst, OPmat4 a )
- OPmat4 OPmat4Interpolate ( OPmat4 a, OPmat4 b, OPfloat percent )
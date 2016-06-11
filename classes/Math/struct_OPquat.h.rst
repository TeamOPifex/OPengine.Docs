OPquat.h
=========

OPquat
----------------
- OPfloat x
- OPfloat y
- OPfloat z
- OPfloat w
Globals
----------------
- const OPquat OPQUAT_IDENTITY
Functions
----------------
- OPquat OPquatCreate ( OPfloat x, OPfloat y, OPfloat z, OPfloat w )
- OPquat OPquatCreate ( OPvec3 axis, OPfloat w )
- OPquat OPquatAdd ( OPquat a, OPquat b )
- OPquat OPquatSub ( OPquat a, OPquat b )
- OPquat OPquatMul ( OPquat a, OPquat b )
- OPquat OPquatScl ( OPquat a, OPfloat s )
- OPquat OPquatConj ( OPquat a )
- OPquat OPquatNorm ( OPquat a )
- OPfloat OPquatLen ( OPquat a )
- OPfloat OPquatDot ( OPquat a, OPquat b )
- OPfloat OPquatAngularDif ( OPquat a, OPquat b )
- OPquat OPquatCreateRot ( OPvec3 axis, OPfloat angle )
- OPquat OPquatCreateLookAt ( OPvec3 eye, OPvec3 target )
- OPvec3 OPquatRot ( OPquat q, OPvec3 v )
- OPvec3 OPquatForward ( OPquat a )
- OPvec3 OPquatUp ( OPquat a )
- OPvec3 OPquatRight ( OPquat a )
- OPquat OPquatRotationBetween ( OPvec3 start, OPvec3 dest )
- OPvec3 OPvec3Orthogonal ( OPvec3 v )
- OPquat OPquatRotationBetween2 ( OPvec3 start, OPvec3 dest )
- OPquat OPquatRotationBetween3 ( OPvec3 start, OPvec3 dest )
- OPquat OPquatRotationBetween4 ( OPvec3 from, OPvec3 to )
- OPquat OPquatRotationBetween5 ( OPvec3 normal )
- OPquat OPquatLerp ( OPquat a, OPquat b, OPfloat p )
OPvec4.h
=========

OPvec4
----------------
-  

----------------
- OPfloat x
- OPfloat y
- OPfloat z
- OPfloat w
Globals
----------------
- const OPvec4 OPVEC4_ZERO
- const OPvec4 OPVEC4_ONE
Functions
----------------
- OPvec4 OPvec4Create ( OPfloat x, OPfloat y, OPfloat z, OPfloat w )
- void OPvec4Add ( OPvec4* dst, OPvec4* a, OPvec4* b )
- void OPvec4Sub ( OPvec4* dst, OPvec4* a, OPvec4* b )
- void OPvec4Mul ( OPvec4* dst, OPvec4* a, OPvec4* b )
- void OPvec4Scl ( OPvec4* dst, OPvec4* a, OPfloat s )
- void OPvec4Div ( OPvec4* dst, OPvec4* a, OPvec4* b )
- void OPvec4Div ( OPvec4* dst, OPvec4* a, OPfloat b )
- OPvec4 OPvec4Create ( OPfloat x )
- OPvec4 OPvec4Create ( OPvec3 xyz, OPfloat w )
- OPvec4 OPvec4Norm ( OPvec4 a )
- OPfloat OPvec4Dot ( OPvec4 a, OPvec4 b )
- OPfloat OPvec4Len ( OPvec4 a )
- OPfloat OPvec4Dist ( OPvec4 a, OPvec4 b )
- OPvec4 OPvec4Read ( OPstream* str )
- void OPvec4Write ( OPvec4 v, OPstream* str )
- OPvec4 OPvec4randNorm (  )
- void OPvec4Log ( const OPchar* m, OPvec4 v )
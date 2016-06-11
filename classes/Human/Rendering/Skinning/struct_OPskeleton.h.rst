OPskeleton.h
=========

OPskeleton
----------------
- ui16 hierarchyCount
- i16* hierarchy
- OPchar* jointNames
- OPmat4* globalPoses
- OPmat4* globalInvPoses
- OPmat4* localPoses
- OPmat4* skinned
Globals
----------------
Functions
----------------
- OPskeleton* OPskeletonCreate ( i16* hierarchy, OPmat4* pose, i32 count, OPchar* names )
- void OPskeletonUpdate ( OPskeleton* skeleton )
- i16 OPskeletonGet ( OPskeleton* skeleton, const OPchar* name )
- void OPskeletonDestroy ( OPskeleton* skeleton )
- OPskeleton* OPskeletonCopy ( OPskeleton* source )
- OPmat4 OPskeletonLocal ( OPskeleton* skeleton, const OPchar* name )
- OPvec3 OPskeletonLocalTranslate ( OPskeleton* skeleton, i16 ind )
- OPvec3 OPskeletonLocalTranslate ( OPskeleton* skeleton, const OPchar* name )
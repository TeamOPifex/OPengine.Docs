OPboundingBox3D.h
=========

OPboundingBox3D
----------------
- OPvec3 min
- OPvec3 max
Globals
----------------
Functions
----------------
- OPboundingBox3D OPboundingBox3DCreate ( OPvec3 min, OPvec3 max )
- void OPboundingBox3DAddVec3 ( OPboundingBox3D* bb, OPvec3* point )
- OPint OPboundingBox3DContainsVec3 ( OPboundingBox3D* bb, OPvec3* point )
- OPint OPboundingBox3DContainsBoundingBox3D ( OPboundingBox3D* bb, OPboundingBox3D* bb2 )
- OPint OPboundingBox3DCollisionBoundingBox3D ( OPboundingBox3D modelBounds, OPboundingBox3D playerBounds )
- i8 OPboundingBox3DRay3D ( OPboundingBox3D b, OPray3D ray )
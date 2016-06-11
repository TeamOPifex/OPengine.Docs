OPcam.h
=========

OPcam
----------------
- OPvec3 pos
- OPvec3 target
- OPvec3 up
- OPfloat fov
- OPfloat aspect
- OPfloat nearView
- OPfloat farView
- OPmat4 proj
- OPmat4 view
Globals
----------------
Functions
----------------
- OPcam OPcamPersp ( OPvec3 position, OPvec3 target, OPvec3 up, OPfloat zNear, OPfloat zFar, OPfloat fov, OPfloat aspect )
- OPcam OPcamOrtho ( OPvec3 position, OPvec3 target, OPvec3 up, OPfloat zNear, OPfloat zFar, OPfloat left, OPfloat right, OPfloat bottom, OPfloat top )
- OPray3D OPcamUnproject ( OPcam* cam, i32 x, i32 y )
- void OPcamUpdateView ( OPcam* cam )
- void OPcamUpdateProj ( OPcam* cam )
- void OPcamUpdate ( OPcam* cam )
- void OPcamBind ( OPcam* camera )
OPphysics.h
=========

OPphysicsScene
----------------
- void* scene
- ui64 elapsed
OPphysicsActor
----------------
OPphysicsStatic
----------------
OPphysicsDynamic
----------------
Globals
----------------
Functions
----------------
- void OPphysicsAddTorque ( OPphysicsDynamic* dynamic, f32 x, f32 y, f32 z )
- void OPphysicsSetAngularVelocity ( OPphysicsDynamic* dynamic, f32 x, f32 y, f32 z )
- void* OPphysicsCreatePlane ( OPphysicsScene* scene )
- void OPphysicsStep ( OPphysicsScene* scene, ui64 elapsed )
- OPphysicsDynamic* OPphysicsCreateBoxDynamic ( OPphysicsScene* scene, f32 x, f32 y, f32 z, f32 sx, f32 sy, f32 sz )
- void OPphysicsGetTransform ( OPphysicsActor* actor, OPmat4* mat )
- void OPphysicsDestroy ( OPphysicsScene* scene )
- OPphysicsScene* OPphysicsCreateScene (  )
- void OPphysicsSetLinearVelocity ( OPphysicsDynamic* dynamic, f32 x, f32 y, f32 z )
- void OPphysicsAddForce ( OPphysicsDynamic* dynamic, f32 x, f32 y, f32 z )
- OPphysicsDynamic* OPphysicsCreateSphereDynamic ( OPphysicsScene* scene, f32 x, f32 y, f32 z, f32 s )
- OPphysicsStatic* OPphysicsCreateSphereStatic ( OPphysicsScene* scene, f32 x, f32 y, f32 z, f32 s )
- OPphysicsStatic* OPphysicsCreateBoxStatic ( OPphysicsScene* scene, f32 x, f32 y, f32 z, f32 sx, f32 sy, f32 sz )
- void OPphysicsShutdown (  )
- void OPphysicsInit (  )
OPsprite3D.h
=========

OPsprite3D
----------------
- OPvec3 Position
- OPvec3 Rotation
- OPvec3 Scale
- OPint Direction
- OPsprite* Sprites
- OPsprite* CurrentSprite
- OPfloat FrameRate
- OPint CurrentFrame
- ui64 CurrentElapsed
- OPint Loop
- OPeffect* Effect
Globals
----------------
Functions
----------------
- void OPsprite3DInit ( OPeffect* effect )
- OPsprite3D* OPsprite3DCreate ( OPsprite* sprites, OPeffect* effect )
- void OPsprite3DCreateFill ( OPsprite3D* sprite, OPsprite* sprites, OPeffect* effect )
- void OPsprite3DDestroy ( OPsprite3D* sprite )
- void OPsprite3DUpdate ( OPsprite3D* sprite, ui64 elapsed )
- void OPsprite3DSetSprite ( OPsprite3D* sprite, i32 index )
- void OPsprite3DPrepReRender ( OPsprite3D* sprite, OPvec3 offset, OPfloat rotation )
- void OPsprite3DPrepRender ( OPsprite3D* sprite, OPcam* camera, OPvec3 offset, OPfloat rotation )
- void OPsprite3DRender ( OPsprite3D* sprite, OPcam* camera )
- void OPsprite3DRenderOffsetRot ( OPsprite3D* sprite, OPcam* camera, OPvec3 offset, OPfloat rotation )
- OPvec2 OPsprite3DSize ( OPsprite3D* sprite )
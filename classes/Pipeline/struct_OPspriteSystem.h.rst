OPspriteSystem.h
=========

OPspriteSystemSprite
----------------
- OPvec2 Position
- OPvec2 Scale
- OPvec2 Center
- OPfloat Rotation
- OPuint CurrentSprite
- OPint CurrentFrame
- OPuint CurrentElapsed
- OPint Direction
OPspriteSystem
----------------
- OPmesh _mesh
- OPspriteSystemSprite* SystemSprites
-  Align
- OPuint Count
- OPuint CountMax
- OPfloat FrameRate
- OPsprite* Sprites
- OPeffect* Effect
- i8 ExternalEffect
Globals
----------------
Functions
----------------
- void OPspriteSystemEffectDefault ( OPeffect* effect )
- void OPspriteSystemInit ( OPspriteSystem* system, OPsprite* sprites, OPint count, OPeffect* effect,  alignment )
- OPspriteSystem* OPspriteSystemCreate ( OPsprite* sprites, OPint count, OPeffect* effect,  alignment )
- OPspriteSystemSprite* OPspriteSystemAdd ( OPspriteSystem* system )
- void OPspriteSystemRemove ( OPspriteSystem* system, OPspriteSystemSprite* sprite )
- void OPspriteSystemUpdate ( OPspriteSystem* system, OPtimer* timer )
- void OPspriteSystemRender ( OPspriteSystem* system, OPcam* camera )
- void OPspriteSystemDestroy ( OPspriteSystem* system )
- OPsprite* OPspriteSystemCurrent ( OPspriteSystem* system, OPspriteSystemSprite* sprite )
- OPboundingBox3D OPspriteSystemBoundingBox3D ( OPspriteSystem* system, OPspriteSystemSprite* sprite )
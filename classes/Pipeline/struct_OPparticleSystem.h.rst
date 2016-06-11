OPparticleSystem.h
=========

OPparticle
----------------
- OPvec3 Position
- OPvec3 Velocity
- OPfloat Angle
- OPfloat AngularVelo
- ui64 Life
- ui64 MaxLife
- OPvec4 Tint
- OPsprite* Animation
- ui8 CurrentFrame

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

OPparticleSys
----------------
- OPentHeap* heap
- OPparticle* particles
- OPtexture* texture
- OPeffect* effect
- OPvec2 uvScale
- OPfloat fps
- OPfloat timeElapsed
Globals
----------------
Functions
----------------
- void OPparticleUpdate ( OPparticle* p, OPtimer* timer )
- void OPparticleSysSpawn ( OPparticleSys* sys, OPparticle particle )
- void OPparticleSysInit ( OPeffect* effect )
- OPparticleSys* OPparticleSysCreate ( OPtexture* texture, ui16 count, OPeffect* effect )
- void OPparticleSysUpdate ( OPparticleSys* sys, OPtimer* timer )
- void OPparticleSysDestroy ( OPparticleSys* sys )
- void OPparticleSysDraw ( OPparticleSys* sys, OPcam* cam, void() ParticleTransform )
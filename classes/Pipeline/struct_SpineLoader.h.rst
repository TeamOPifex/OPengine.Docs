SpineLoader.h
=========

Spine
----------------
Globals
----------------
Functions
----------------
- void SpineAddLoader (  )
- void SpineInitialize (  )
- void SpineSetMix ( Spine* spine, const OPchar* from, const OPchar* to, f32 duration )
- void SpineSetAnim ( Spine* spine, i32 track, const OPchar* anim, OPint loop )
- void SpineAddAnim ( Spine* spine, i32 track, const OPchar* anim, OPint loop, OPfloat delay )
- void SpineBuildMixingState ( Spine* spine )
- i32 SpineLoad ( const OPchar* filename, Spine* spine )
- void SpineRender ( Spine* spine, OPmat4* world, OPeffect* effect, OPcam* camera )
- void SpineUpdate ( Spine* spine, OPtimer* timer )
- i32 SpineUnload ( void* spine )
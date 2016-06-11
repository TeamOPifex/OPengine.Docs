OPskeletonAnimationTransition.h
=========

OPskeletonAnimationTransition
----------------
- OPskeletonAnimation* Start
- OPskeletonAnimation* End
- OPfloat Duration
- OPfloat Current
Globals
----------------
Functions
----------------
- OPskeletonAnimationTransition OPskeletonAnimationTransitionInit ( OPskeletonAnimation* start, OPskeletonAnimation* end, OPfloat duration )
- OPint OPskeletonAnimationTransitionUpdate ( OPskeletonAnimationTransition* transition, OPtimer* timer )
- void OPskeletonAnimationTransitionApply ( OPskeletonAnimationTransition* transition, OPskeleton* skeleton )
- void OPskeletonAnimationTransitionReset ( OPskeletonAnimationTransition* transition )
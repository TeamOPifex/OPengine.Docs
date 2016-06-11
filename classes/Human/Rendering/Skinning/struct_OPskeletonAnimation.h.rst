OPskeletonAnimation.h
=========

OPskeletonAnimation
----------------
- OPskeleton* Skeleton
- OPmat4* JointFrames
- OPuint FrameCount
- OPuint Frame
- ui64 Elapsed
- ui64 FramesPer
- OPmat4* CurrentFrame
- OPint BoneCount
- OPint Loop
- OPuint LoopsCompleted
- OPuint LastFrame
- OPskeletonAnimationEvent* Events
- OPuint EventCount
OPskeletonAnimationEvent
----------------
- void() Event
- OPuint Frame
- OPuint End
- OPint OnFrameChange
Globals
----------------
Functions
----------------
- void OPskeletonAnimationInit ( OPskeletonAnimation* skelAnim, OPint boneCount, OPmat4* frames, i32 count )
- OPskeletonAnimation* OPskeletonAnimationCreate ( OPint boneCount, OPmat4* frames, OPuint count )
- void OPskeletonAnimationUpdate ( OPskeletonAnimation* skelAnim, OPtimer* timer, OPfloat timeScale )
- void OPskeletonAnimationUpdate ( OPskeletonAnimation* skelAnim, OPtimer* timer )
- void OPskeletonAnimationUpdateEvents ( OPskeletonAnimation* skelAnim, void* data )
- void OPskeletonAnimationApply ( OPskeletonAnimation* skelAnim, OPskeleton* skeleton )
- void OPskeletonAnimationApply ( OPskeletonAnimation* skelAnim, OPskeleton* skeleton, i16 fromJoint )
- void OPskeletonAnimationApply ( OPmat4* animationFrame, OPskeleton* skeleton )
- void OPskeletonAnimationApply ( OPmat4* animationFrame, OPskeleton* skeleton, i16 fromJoint )
- void OPskeletonAnimationMerge ( OPskeletonAnimation* skelAnim1, OPskeletonAnimation* skelAnim2, OPfloat merge )
- void OPskeletonAnimationCombine ( OPskeletonAnimation* skelAnim, OPskeletonAnimation* skelAnim2, OPskeleton* skeleton, i16 fromJoint )
- void OPskeletonAnimationSetEvents ( OPskeletonAnimation* skelAnim, OPuint frames, OPskeletonAnimationEvent* events )
- void OPskeletonAnimationReset ( OPskeletonAnimation* skelAnim )
- OPskeletonAnimation* OPskeletonAnimationCopy ( OPskeletonAnimation* source, OPint boneCount )
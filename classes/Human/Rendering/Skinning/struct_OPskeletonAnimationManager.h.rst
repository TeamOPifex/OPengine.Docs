OPskeletonAnimationManager.h
=========

OPskeletonAnimationMix
----------------
-  animations
-  mergeJoints

.. epigraph::
	.. raw:: html

		Mixes animations together<br />

OPskeletonAnimationManagerTransition
----------------
- OPskeletonAnimation* animation
- OPfloat transitionTime

.. epigraph::
	.. raw:: html

		A transition animation grouping<br />

OPskeletonAnimationManager
----------------
- OPskeleton* skeleton
- i16 animationIndex
-  animations
-  animationJointMix
- OPskeletonAnimationManagerTransition transition
- OPskeletonAnimationManagerTransition buffer
- OPfloat currentTime

.. epigraph::
	.. raw:: html

		The manager itself, which will automatically merge and play animations appropriately<br />

Globals
----------------
Functions
----------------
- void OPskeletonAnimationManagerInit ( OPskeletonAnimationManager* manager, OPskeleton* skeleton )
- OPskeletonAnimationManager* OPskeletonAnimationManagerCreate ( OPskeleton* skeleton )
- void OPskeletonAnimationManagerSet ( OPskeletonAnimationManager* manager, OPskeletonAnimation* animation )
- void OPskeletonAnimationManagerMix ( OPskeletonAnimationManager* manager, OPskeletonAnimation* animation, i16 fromJoint )
- void OPskeletonAnimationManagerTransition ( OPskeletonAnimationManager* manager, OPskeletonAnimation* animation, OPfloat duration )
- void OPskeletonAnimationManagerUpdate ( OPskeletonAnimationManager* manager, OPtimer* timer, OPfloat timeScale )
- void OPskeletonAnimationManagerUpdate ( OPskeletonAnimationManager* manager, OPtimer* timer )
- void OPskeletonAnimationManagerDestroy ( OPskeletonAnimationManager* manager )
- void OPskeletonAnimationManagerFree ( OPskeletonAnimationManager* manager )
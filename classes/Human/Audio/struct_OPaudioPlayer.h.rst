OPaudioPlayer.h
=========

OPaudioPlayer
----------------
- OPaudioEmitter* Emitters
- OPint Count
- OPint Current
Globals
----------------
- OPaudioPlayer* OPAUD_CURR_PLAYER

.. epigraph::
	.. raw:: html

		_____ _ _ _<br />/ ____| | | | | |<br />| | __| | ___ | |__ __ _| |___<br />| | |_ | |/ _ \| '_ \ / _` | / __|<br />| |__| | | (_) | |_) | (_| | \__ \<br />\_____|_|\___/|_.__/ \__,_|_|___/<br />

Functions
----------------
- OPaudioPlayer OPaudPlayerCreate ( OPaudioSource* src, OPint sounds, OPint looping )

.. epigraph::
	.. raw:: html

		______ _ _<br />____| | | (_)<br />|__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />__| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | |_| | | | | (__| |_| | (_) | | | \__ \<br />\__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- void OPaudPlayerDestroy ( OPaudioPlayer* player )
- void OPaudPlayerPlay (  )
- void OPaudPlayerStop (  )
- void OPaudPlayerPause (  )
- void OPaudPlayerUpdate ( void() Proc )
- void OPaudPlayerPosition ( OPvec3* position )
- void OPaudPlayerVelocity ( OPvec3* velocity )
- void OPaudPlayerVolume ( OPfloat gain )
- void OPaudPlayerPitch ( OPfloat pitch )
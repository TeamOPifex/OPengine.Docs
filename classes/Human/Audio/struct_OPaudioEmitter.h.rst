OPaudioEmitter.h
=========

OPaudioEmitter
----------------

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

Globals
----------------
- OPaudioEmitter* OPAUD_CURR_EMITTER

.. epigraph::
	.. raw:: html

		_____ _ _ _<br />/ ____| | | | | |<br />| | __| | ___ | |__ __ _| |___<br />| | |_ | |/ _ \| '_ \ / _` | / __|<br />| |__| | | (_) | |_) | (_| | \__ \<br />\_____|_|\___/|_.__/ \__,_|_|___/<br />

- OPentHeap OPAUD_REG_EMITTERS
- OPthread OPAUD_UPDATE_THREAD
Functions
----------------
- void OPaudInitThread ( OPint maxEmitters )

.. epigraph::
	.. raw:: html

		_ _ ______ _ _ _ ______ _ _<br />/\ | (_) | ____| (_) | | | | ____| | | (_)<br />/ \ _ _ __| |_ ___ | |__ _ __ ___ _| |_| |_ ___ _ __ | |__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />/ /\ \| | | |/ _` | |/ _ \| __| | '_ ` _ \| | __| __/ _ \ '__| | __| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />/ ____ \ |_| | (_| | | (_) | |____| | | | | | | |_| || __/ | | | | |_| | | | | (__| |_| | (_) | | | \__ \<br />/_/ \_\__,_|\__,_|_|\___/|______|_| |_| |_|_|\__|\__\___|_| |_| \__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- OPaudioEmitter* OPaudCreateEmitter ( OPaudioSource* src, OPint flags )
- void OPaudDestroyEmitter ( OPaudioEmitter* emitter )
- OPaudioEmitter* OPaudGetEmitter ( OPaudioSource* src, OPint flags )
- void OPaudRecycleEmitter ( OPaudioEmitter* emitter )
- void OPaudEnqueueBuffer ( ui8* buffer, OPint length )
- void OPaudPlay (  )
- void OPaudPause (  )
- void OPaudStop (  )
- void OPaudSafePlay ( OPaudioEmitter* emitter )
- void OPaudSafePause ( OPaudioEmitter* emitter )
- void OPaudSafeStop ( OPaudioEmitter* emitter )
- OPint OPaudUpdate ( void() Proc )
- OPint OPaudSafeUpdate ( OPaudioEmitter* emitter, void() Proc )
- OPint OPaudProc ( OPaudioEmitter* emitter, void() Proc )
- void OPaudPosition ( OPaudioEmitter* emitter, OPvec3* position )
- void OPaudVelocity ( OPaudioEmitter* emitter, OPvec3* velocity )
- void OPaudVolume ( OPaudioEmitter* emitter, OPfloat gain )
- void OPaudPitch ( OPaudioEmitter* emitter, OPfloat pitch )
- void OPaudProcess ( OPaudioEmitter* emit, OPint length )
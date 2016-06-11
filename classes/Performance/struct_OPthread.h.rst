OPthread.h
=========

OPthread
----------------
- OPint Status
- HANDLE Thread
- DWORD ThreadId
- void* Return

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

OPmutex
----------------
- HANDLE Mutex
Globals
----------------
Functions
----------------
- OPthread OPthreadStart ( void*() function, void* params )
- OPint OPthreadStop ( void* retval )
- OPint OPthreadJoin ( OPthread* thread )
- OPmutex OPmutexCreate (  )
- OPint OPmutexLock ( OPmutex* mutex )
- OPint OPmutexUnlock ( OPmutex* mutex )
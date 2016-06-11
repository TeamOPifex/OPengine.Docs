OPrenderBuffer.h
=========

OPrenderBuffer
----------------
- ui32 Type
- ui32 ElementSize
- OPuint ElementCount
- ui32 Handle

.. epigraph::
	.. raw:: html

		_____ _ _<br />/ ____| | | |<br />| (___ | |_ _ __ _ _ ___| |_ ___<br />\___ \| __| '__| | | |/ __| __/ __|<br />____) | |_| | | |_| | (__| |_\__ \<br />|_____/ \__|_| \__,_|\___|\__|___/<br />

Globals
----------------
- OPrenderBuffer* OPRENDER_CURR_VB

.. epigraph::
	.. raw:: html

		_____ _ _ _<br />/ ____| | | | | |<br />| | __| | ___ | |__ __ _| |___<br />| | |_ | |/ _ \| '_ \ / _` | / __|<br />| |__| | | (_) | |_) | (_| | \__ \<br />\_____|_|\___/|_.__/ \__,_|_|___/<br />

- OPrenderBuffer* OPRENDER_CURR_IB
Functions
----------------
- OPrenderBuffer OPrenderGenBuffer ( ui32 type )

.. epigraph::
	.. raw:: html

		______ _ _<br />____| | | (_)<br />|__ _ _ _ __ ___| |_ _ ___ _ __ ___<br />__| | | | '_ \ / __| __| |/ _ \| '_ \/ __|<br />| | |_| | | | | (__| |_| | (_) | | | \__ \<br />\__,_|_| |_|\___|\__|_|\___/|_| |_|___/<br />

- void OPrenderDelBuffer ( OPrenderBuffer* buff )
- void OPrenderSetBufferData ( OPrenderBuffer* buff, ui32 elementSize, OPuint count, const void* data )
- void OPrenderSetBufferSubData ( OPrenderBuffer* buff, ui32 elementSize, ui32 offsetCount, OPuint count, const void* data )
- void OPrenderBindBuffer ( OPrenderBuffer* buffer )
- void OPrenderDrawBufferIndexed ( ui32 offset )
- void OPrenderDrawBuffer ( ui32 offset )
- void OPrenderDrawIndexed ( ui32 offset, ui32 count )
- void OPrenderDrawUserArray ( void* vertices, ui32 attrs, ui32 offset, ui32 count )